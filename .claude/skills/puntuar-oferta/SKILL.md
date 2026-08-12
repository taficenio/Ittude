---
name: puntuar-oferta
description: Puntuar una oferta de 0-100 en 5 dimensiones para determinar si postular, postular solo con referido, o saltear.
---

# /puntuar-oferta - Motor de Puntuación de Fit de Oferta

## Cuándo Usar

- User pastes a JD and wants to know if they should apply
- User is triaging multiple JDs and needs to prioritize which to pursue
- User asks "is this role worth applying to?" or "should I bother with this one?"
- Before investing time in `/adaptar-cv` or `/carta-presentacion`, run this first to avoid wasted effort

## Entradas

- **Required:** Job description text (pasted or referenced)
- **Auto-loaded:** `biblioteca-contexto/biblioteca-experiencias.md` (skills and experience to match against)
- **Auto-loaded:** `biblioteca-contexto/plan-carrera.md` (level preference, industry preference, remote/hybrid/onsite preference, dream offer, comp target)
- **Auto-loaded:** `biblioteca-contexto/qa-master.md` (comp expectations if defined there)

If `biblioteca-experiencias.md` or `plan-carrera.md` is empty or contains only template placeholders, STOP and tell the user: "I need your experience library and career plan filled in to score a JD accurately. Without them, every score is a guess. Fill those files first."

## Proceso

### Step 1: Parse the JD
Extract structured data from the job description:
- Company name, role title, level
- Location and remote policy
- Required skills (list each)
- Preferred skills (list each)
- Years of experience required
- Compensation range (if listed)
- Company stage signals (startup language vs enterprise language, funding info)
- Industry and domain
- Team structure mentions (team size, reporting structure)
- Growth signals (new team, greenfield, scaling existing)

### Step 2: Score Dimension 1 -- Skill Match (0-20)
Compare every required and preferred skill against `biblioteca-experiencias.md`:
- For each REQUIRED skill: check if experience library has a direct match (bullet with that skill + metric), partial match (related skill or adjacent experience), or no match
- For each PREFERRED skill: same check
- **Handling vague JD requirements:** Some JDs list broad requirements like "strong product sense" or "experience building 0-to-1 products" without naming specific skills. For vague requirements, look for pattern matches across the experience library rather than keyword matches. Score these as STRONG if the user has 2+ bullets demonstrating the underlying competency, PARTIAL if 1 bullet, NONE if no evidence. Note in the output that the requirement was interpreted broadly.
- **Scoring formula:**
  - Count required skills matched (strong or partial) / total required skills = required_ratio
  - Count preferred skills matched / total preferred skills = preferred_ratio
  - Score = (required_ratio * 14) + (preferred_ratio * 6)
  - Round to nearest integer
- Show the match table in output so the user sees exactly where they match and where they don't


### Step 3: Score Dimension 2 -- Seniority Fit (0-20)
Compare the JD's seniority signals against `plan-carrera.md` level preferences:
- **Years of experience alignment:** Does the user meet the minimum? Within 1 year = full credit. 2+ years short = penalty. Overqualified by 3+ years = slight penalty.
- **Level match:** Does the JD level (IC4, IC5, manager, senior, staff, director) align with plan-carrera.md level preferences? Exact match = full credit. One level below target = partial. Two levels off = low.
- **Scope match:** Does the role scope (own a feature vs own a product line vs own a business unit) match the user's trajectory?

**Career changer seniority adjustment:** If the user has 0 PM-titled years but has PM-adjacent experience (consulting, engineering, design), do NOT score years-of-experience as a flat zero. Instead:
- Count total years of PM-ADJACENT work from `biblioteca-experiencias.md` (e.g., consulting engagement management, engineering product ownership, design leadership) and apply a 0.5x conversion factor. A McKinsey EM with 4 years of product-adjacent consulting work = ~2 equivalent PM years for seniority scoring purposes. This reflects reality: recruiters penalize career changers, but less severely when the adjacent experience directly maps to PM activities (roadmapping, user research, cross-functional leadership, prioritization).
- If the JD requires "3-5 years PM experience" and the user has 0 PM years but 6 years of PM-adjacent work (~3 equivalent years), score as "at the low end of the range" (partial credit), not "2+ years short" (heavy penalty).
- In the output, show the conversion explicitly: "PM-titled years: 0. PM-adjacent years: [N] (from [source]). Effective seniority: ~[N * 0.5] PM-equivalent years. Gap: [JD requirement] - [equivalent years] = [delta]."
- NOTE: This adjustment is for scoring purposes only. In the Skill Match dimension, "X+ years PM experience" requirements with 0 actual PM years should still be scored as NONE with a gap-table note. The seniority dimension captures the LEVEL fit; the skill match dimension captures the TITLE fit. Both matter, but they are different signals.


- **Scoring guide:**
  - 18-20: Exact level and years match, scope aligns with career trajectory
  - 12-17: Close match, one dimension slightly off
  - 6-11: Meaningful mismatch on level or years, but not disqualifying
  - 0-5: Significantly over/under-leveled, years way off


### Step 4: Score Dimension 3 -- Culture Signals (0-20)
Assess culture fit from JD language and plan-carrera.md preferences:
- **Remote/hybrid/onsite match:** Does the JD's work model match the user's preference? Exact match = 5 pts. Acceptable alternative = 3 pts. Dealbreaker mismatch = 0 pts.
- **Company stage match:** Startup vs growth vs enterprise. Does it match plan-carrera.md target companies preference? Match = 5 pts.
- **Industry alignment:** Is this an industry the user listed in plan-carrera.md? Primary industry = 5 pts. Secondary = 3 pts. Not listed = 1 pt.
- **Work style signals:** Does the JD language suggest pace, autonomy, collaboration style that aligns? Look for signals like "fast-paced" (startup energy), "process-oriented" (enterprise), "ambiguity" (early stage), "stakeholder management" (big company). Compare against what the user's career plan implies. 0-5 pts.

**REMOTE-ONLY CANDIDATE SCORING ADJUSTMENT:** If `plan-carrera.md` indicates the user has a remote-only preference or caregiver/family constraints, apply these adjustments to the scoring logic:
- **Location/Logistics penalty:** Any JD that says "onsite," "in-office," or "hybrid required" (not "hybrid optional") gets an automatic **-20 penalty on the Culture Signals dimension** (overriding the work-model sub-score entirely to 0 pts for that component). Additionally, add a prominent WARNING flag in the output: "REMOTE MISMATCH: This role requires [onsite/hybrid]. Your career plan specifies remote-only. This is likely a dealbreaker."
- **"Remote-friendly" or "flexible" language:** No penalty, but note the ambiguity in the Culture Signals section: "JD says '[exact language].' This could mean fully remote or hybrid-with-flexibility. Confirm the actual policy before investing application time."
- **"Remote Infrastructure" positive signal:** If the JD mentions distributed-first culture signals (async communication tools, "work from anywhere," no "collaborative office environment" or "in-person collaboration" language, mentions of GitLab-style handbook-first approach, or companies known for distributed-first culture like GitLab, Automattic, Zapier), add a +2 bonus to the Culture Signals dimension and note: "Remote Infrastructure: Strong distributed-first signals detected."
- **No penalty for the remote preference itself.** Remote-only is a logistics preference, not a weakness. Do not reduce any other dimension score because the user prefers remote work.

### Step 5: Score Dimension 4 -- Comp Range (0-20)
Assess compensation alignment:
- **If JD lists comp range:** Compare against the user's comp target from plan-carrera.md or qa-master.md
  - Range midpoint within 10% of target = 18-20
  - Range midpoint within 20% = 12-17
  - Range midpoint 20%+ below target = 6-11
  - Range clearly below minimum acceptable = 0-5
- **If JD does NOT list comp range:** Estimate based on:
  - Company stage (public, late-stage, early-stage)
  - Location (SF, NYC, remote adjustments)
  - Role level
  - Industry norms
  - Note the estimate confidence level (high/medium/low)
  - Score based on estimated range vs target, but cap maximum score at 15 (uncertainty penalty)
- **If JD does NOT list comp range AND company is private with no public comp data (no Glassdoor, levels.fyi, or Blind data):**
  - Estimate from: comparable companies at the same stage and funding level, similar role postings that DO list comp, and location-based market data for the role level
  - Set confidence to LOW
  - Cap maximum score at 12 (higher uncertainty penalty)
  - State explicitly in output: "No comp data available for [Company]. Estimate is based on [comparable companies used]. Treat this score with caution and run /investigar-salario before negotiating."
  - If even comparable-company estimation is unreliable (e.g., very early stage, no funding data, niche industry), score the dimension at 10 and note: "Comp dimension scored at default 10/20 due to insufficient data. This is neither positive nor negative -- it reflects genuine uncertainty. Run /investigar-salario to resolve."

**Pay-cut scenario advisory:** If the user's CURRENT comp (from plan-carrera.md or biblioteca-experiencias.md) is higher than the estimated or listed comp range for this role, add a `PAY-CUT ADVISORY` to the Comp Range section of the output: "Your current TC of $[X] is above the estimated range for this role ($[low]-$[high]). This is a pay-cut move. This is NOT a negative signal -- it may reflect deliberate downleveling, a career change, or a values-driven move. But confirm the trade-off is intentional before investing application time. Run /investigar-salario and /negociar before accepting any offer at this company."

**Cross-market comp advisory:** If the user's current comp is in a non-US market and the role is in the US (or vice versa), do NOT compare raw numbers. Instead note: "Your current comp is in [market]. Direct numeric comparison to [target market] is misleading due to market, tax, and cost-of-living differences. The Comp Range score is based on how the JD's range compares to your TARGET comp ($[target from career-plan]), not your current comp."

### Step 6: Score Dimension 5 -- Growth Trajectory (0-20)
Assess whether this role moves the user toward their #1 career preference or sideways:
- Read the user's dream offer from plan-carrera.md
- Read the user's level preferences (ranked 1-3)
- **Toward dream offer:** Does this role build skills, domain expertise, or resume signal that gets closer to the dream offer? If yes, high score.
- **Lateral move:** Same level, same type of work, different company but no strategic advantage. Medium score.
- **Away from trajectory:** Role is in a different function, different seniority direction, or industry that doesn't connect to the user's stated goals. Low score.
- **Scoring guide:**
  - 18-20: This role IS the dream offer, or is a direct stepping stone (same company tier, same domain, levels up)
  - 12-17: Builds relevant skills or brand signal, even if not the exact dream role
  - 6-11: Lateral move. Pays bills but doesn't advance the career plan.
  - 0-5: Actively moves away from stated trajectory

**EARLY-CAREER DIMENSION WEIGHTING:** For candidates with < 3 years total experience OR APM/Associate-level titles (detected from plan-carrera.md), adjust the standard scoring:
- Reduce Skill Match weight to 15% (JD years-of-experience requirements will always penalize early-career candidates — this dimension should not dominate the score since the real question is transferable skill quality, not years)
- Increase Growth Trajectory to 30% (the most important question for an early-career candidate is: does this role accelerate my career toward my dream offer? A lateral move at year 1.5 is a much bigger waste than at year 10)
- Seniority Fit 15% (early-career candidates will almost always be "under-experienced" on paper — weighting this heavily penalizes them unfairly when many companies hire stretch candidates at this level)
- Comp Range 20%, Culture Signals 15% (Location match is folded into Culture Signals as the remote/hybrid/onsite sub-score — it is NOT a separate dimension. The 5% reduction in Culture Signals reflects that early-career candidates are generally more location-flexible.)
- **Weighted scoring mechanics:** Score each dimension on the standard 0-20 scale using the existing rubrics. Then compute the weighted total: `Total = (Skill × 0.75) + (Seniority × 0.75) + (Culture × 0.75) + (Comp × 1.0) + (Growth × 1.5)` = max 95 raw. Normalize to 0-100 by multiplying by (100/95): `Final Score = Raw Total × 1.053`. Display the raw dimension scores in the output table as "[X]/20" alongside the effective weighted contribution (e.g., "Skill Match: 14/20 (weighted: 10.5/15)"). This ensures the sub-dimension rubrics remain consistent while the weights correctly shift emphasis. The normalization preserves the 60/75 recommendation thresholds on the 0-100 scale.
- Add a "Stretch Role" qualifier: if the JD requires [X] years and the candidate has fewer than [X-2] years (gap of 1-3 years), do NOT auto-penalize to zero on Seniority Fit. Instead, score based on scope match (did the candidate's output match the described scope?). Many companies list "3-5 years" but regularly hire strong candidates with 1.5-2 years. Flag: "STRETCH ROLE: JD requests [X] years but your output metrics suggest scope-readiness. Apply if other dimensions are strong — companies regularly hire below their posted experience threshold at this level." **Threshold:** Stretch Role applies when the experience gap is 1-3 years. Gaps of 4+ years revert to standard seniority penalty — a JD requiring 7+ years is not a stretch role for a candidate with 1.5 years.
- **Interaction with career changer adjustment:** Early-career weighting and the career changer seniority adjustment (0.5x conversion) are mutually exclusive. If the candidate has < 3 years in their current function but prior experience in another function, apply the career changer adjustment to calculate PM-equivalent years first, THEN check if the adjusted total is still < 3 years to determine whether early-career weighting applies.

**EXECUTIVE-LEVEL DIMENSION WEIGHTING:** For VP/Director+ candidates (detected from plan-carrera.md), adjust the standard scoring:
- Reduce Skill Match weight to 15% (at this level, specific keyword matches matter less than strategic fit)
- Increase Culture Signals to 30% (reporting line, org structure, board dynamics matter enormously)
- Seniority Fit 20%, Comp Range 25%, Location 10%
- Add a "Strategic Scope" qualifier: does the JD describe VP-level scope (P&L ownership, team building, strategy setting) or is it a glorified Senior PM role with a VP title? If the JD title says VP/Director but the scope description matches Senior IC work (owns a single feature, no direct reports, no budget authority), flag: "TITLE INFLATION WARNING: This JD has a [VP/Director] title but describes [Senior PM]-level scope. Score the Seniority Fit dimension based on actual scope, not title. This mismatch may indicate the company uses inflated titles, which affects long-term career trajectory."

### Step 7: Calculate Total and Recommendation
Sum all 5 dimension scores.

**Visa / work authorization check (runs before dealbreaker check):** If `plan-carrera.md` or `qa-master.md` indicates the user needs visa sponsorship (H-1B, work permit, etc.), add a **Visa Sponsorship** advisory section to the output. This is NOT a scored dimension (it does not affect the 0-100 score) but it IS a critical filter:
- Check if the JD explicitly mentions visa sponsorship policy ("must be authorized to work," "will not sponsor," "sponsorship available").
- Cross-reference `empresas-objetivo.md` for confirmed sponsorship history.
- If the JD says "will not sponsor" or "must be authorized to work in [country] without sponsorship," flag: "SKIP (VISA DEALBREAKER): This role explicitly does not offer visa sponsorship." Override the recommendation to SKIP regardless of score.
- If the JD is silent on sponsorship but the company has confirmed sponsorship history in `empresas-objetivo.md`, note: "JD does not mention sponsorship. [Company] has a track record of H-1B sponsorship ([N] petitions per USCIS data). Proceed but confirm sponsorship availability for this specific role in the recruiter screen."
- If the JD is silent and no sponsorship data exists, flag: "VISA RISK: No sponsorship information available. Verify before investing time in the application. Check h1bdata.info or myvisajobs.com."
- For users needing sponsorship who are comparing current non-US comp to US comp ranges, note the market difference in the Comp Range dimension: "User's current comp is in a non-US market ([currency/location]). The Comp Range score is based on the US market rate for this role, not a comparison to current comp."

**Dealbreaker check (runs before applying recommendation thresholds):** Check `plan-carrera.md` for any stated dealbreakers (e.g., "NOT willing to relocate to X," "minimum comp $Y," "will not consider roles below Z level"). If the JD triggers a dealbreaker, override the total score recommendation to SKIP regardless of the numeric score. Display the total score for reference but mark: "SKIP (DEALBREAKER: [reason]). Score of [X] would otherwise suggest [recommendation], but this role conflicts with a stated non-negotiable."

Apply recommendation:
- **Below 60: SKIP.** Explain the top 2 reasons it doesn't fit. Time is better spent elsewhere.
- **60-74: APPLY WITH REFERRAL ONLY.** The gaps mean a cold application will likely fail. A referral compensates for the mismatch. Identify which gaps the referral needs to cover.
- **75-100: APPLY IMMEDIATELY.** Strong match. Prioritize this application. Note any minor gaps to address in resume/cover letter.

**Boundary case handling:** A score of exactly 60 falls in the APPLY WITH REFERRAL ONLY band. A score of exactly 75 falls in the APPLY IMMEDIATELY band. When a score lands on a boundary, note it explicitly: "Score of [60/75] is at the boundary between [X] and [Y]. Given [strongest dimension or weakest dimension], the recommendation is [X]." If the user's weakest dimension is Comp Range or Seniority Fit (hard-to-overcome gaps), lean toward the lower recommendation. If the weakest dimension is Culture Signals or Growth Trajectory (softer factors), lean toward the higher recommendation.

## Salida

```markdown
## Job Fit Score - [Company Name] [Role Title]

### Total Score: [XX]/100 -- [SKIP | APPLY WITH REFERRAL ONLY | APPLY IMMEDIATELY]

| Dimension | Score | Key Factor |
|-----------|-------|------------|
| Skill Match | [X]/20 | [one-line summary] |
| Seniority Fit | [X]/20 | [one-line summary] |
| Culture Signals | [X]/20 | [one-line summary] |
| Comp Range | [X]/20 | [one-line summary] |
| Growth Trajectory | [X]/20 | [one-line summary] |

---

### Skill Match Breakdown ([X]/20)

| JD Requirement | Type | Match | Source |
|---------------|------|-------|--------|
| [skill 1] | Required | STRONG | [experience-library bullet reference] |
| [skill 2] | Required | PARTIAL | [what you have vs what they want] |
| [skill 3] | Required | NONE | [gap] |
| [skill 4] | Preferred | STRONG | [experience-library bullet reference] |
[... all skills ...]

Required match rate: [X]/[Y] ([Z]%)
Preferred match rate: [X]/[Y] ([Z]%)

### Seniority Fit ([X]/20)
- JD level: [extracted level]
- Your target level: [from career-plan]
- Years required: [JD] vs yours: [actual]
- Assessment: [explanation]

### Culture Signals ([X]/20)
- Work model: JD says [X], you prefer [Y] -- [match/mismatch]
- Company stage: [X] -- [match/mismatch]
- Industry: [X] -- [primary/secondary/unlisted]
- Work style: [assessment based on JD language]

### Comp Range ([X]/20)
- JD range: [listed or "Not listed - estimated [range] at [confidence]"]
- Your target: [from career-plan]
- Assessment: [within range / below / above]

### Growth Trajectory ([X]/20)
- Dream offer: [from career-plan]
- This role: [how it connects or doesn't]
- Assessment: [stepping stone / lateral / divergent]

---

### Domain Valence Indicator
**Domain experience: [ASSET / NEUTRAL / LIABILITY] for this role.**
[1-sentence explanation. E.g., "Your 6 years of healthcare PM experience is an ASSET — the JD explicitly requires health-tech domain knowledge." OR "Your fintech background is NEUTRAL — the role is domain-agnostic and cares about PM craft, not industry expertise." OR "Your defense industry background is a LIABILITY — the company is a consumer social app with no overlap, and your employer brands may not register with their recruiters. Mitigate with a work product and referral."]

### Recommendation
[2-3 sentences explaining the score and what to do next. If APPLY, suggest next step (/adaptar-cv or /pedir-referido). If SKIP, suggest what to look for instead.]
```

## Ejemplo

**Input:**
```
/puntuar-oferta

Senior Product Manager, AI Platform - Notion
Requirements: 6+ years PM experience, AI/ML product experience,
platform/API experience, cross-functional leadership, data-driven
decision making. Preferred: B2B SaaS, user research, SQL.
Hybrid in SF. Comp: $200K-$280K base.
```

**Output:**
```markdown
## Job Fit Score - Notion Senior PM, AI Platform

### Total Score: 72/100 -- APPLY WITH REFERRAL ONLY

| Dimension | Score | Key Factor |
|-----------|-------|------------|
| Skill Match | 14/20 | Strong on 5/8 skills, gap on platform/API and years |
| Seniority Fit | 13/20 | 4 years PM vs 6+ required; strong scope match |
| Culture Signals | 18/20 | SF hybrid matches; B2B SaaS + AI industry match |
| Comp Range | 16/20 | $200-280K base aligns with $350K+ total target |
| Growth Trajectory | 11/20 | AI domain builds toward dream, but platform ≠ core growth PM path |

---

### Skill Match Breakdown (14/20)

| JD Requirement | Type | Match | Source |
|---------------|------|-------|--------|
| AI/ML product experience | Required | PARTIAL | "AI recommendation engine" -- usage, not platform-building |
| 6+ years PM experience | Required | NONE | 4 years PM + 2 years consulting |
| Platform/API experience | Required | NONE | No platform PM experience in library |
| Cross-functional leadership | Required | STRONG | "Led 8-person cross-functional team" |
| Data-driven decision making | Required | STRONG | "Built A/B testing framework, 40+ experiments" |
| B2B SaaS | Preferred | STRONG | "3 years B2B SaaS products" |
| User research | Preferred | STRONG | "60+ user research interviews" |
| SQL | Preferred | STRONG | "Own SQL dashboards for funnel monitoring" |

Required match rate: 2/5 (40%)
Preferred match rate: 3/3 (100%)

[... remaining dimension details ...]

### Recommendation
At 72, this is borderline -- strong skill overlap on the preferred qualifications but real gaps on years and platform experience. A cold application will likely get filtered by the years requirement. Get a referral who can vouch for your trajectory and impact per year. Next step: `/pedir-referido` if you have a Notion connection, or `/solicitud-conexion` to build one.
```

## Verificaciones de Calidad

**Good output looks like:**
- Every score has a clear justification, not just a number
- Skill match table shows the full breakdown so the user sees exactly where they stand
- Comp estimate (when JD doesn't list range) states confidence level and reasoning
- Recommendation gives actionable next steps, not just "apply" or "don't apply"
- Growth trajectory references the user's actual dream offer and career plan, not generic career advice
- Scores are honest. A 90+ score should be rare. Most real-world JDs will score 55-80.
- **Score inflation guard:** After computing the total, run a sanity check. If a required skill match rate is below 50% but the total score is above 70, something is wrong -- recheck the scoring. If the user has 0 matches on 2+ required skills, the total should almost never exceed 65 regardless of how strong other dimensions are. A clearly bad match (wrong level, wrong function, missing most requirements) should score 40-50, not 60+. The formulas are designed to prevent this, but verify the math before presenting.

**Bad output looks like:**
- Scores without justification ("Skill Match: 16/20" with no breakdown)
- Inflated scores to make the user feel good (everything is 80+)
- Generic growth trajectory assessment that doesn't reference the user's specific career plan
- Missing comp estimate when JD doesn't list range (just says "Unknown")
- Recommendation that doesn't suggest a specific next action
- Skill match that counts partial matches the same as strong matches

**Persona-specific checks (verify these when applicable):**
- **International/unknown employers:** If the user's experience is from companies unknown in the target market, the Skill Match scoring must evaluate the UNDERLYING experience (scale, metrics, domain) not the brand signal. "5 years at Rakuten Ichiba ($15B GMV)" is a STRONG match for e-commerce requirements even though a US recruiter may not recognize the name. Do not penalize skill match scores because the employer is non-US-famous.
- **Visa-requiring candidates:** The Visa Sponsorship advisory section must always appear in the output when plan-carrera.md indicates visa needs. For companies with confirmed sponsorship in empresas-objetivo.md, include the petition count. For companies not in empresas-objetivo.md, always flag as VISA RISK and provide the research instruction.
- **Cross-market comp:** If the user's current comp is in a non-US currency, the Comp Range dimension must score based on the user's stated US TARGET range (from plan-carrera.md), never by converting current non-US comp to USD. A EUR 130K candidate targeting $280-340K is within normal US Senior PM range -- do not penalize.
- **Remote-only candidate:** If plan-carrera.md indicates remote-only preference: (a) Any JD that says "onsite" or "hybrid required" received a -20 penalty on the Culture Signals / Location dimension AND a prominent WARNING flag. (b) "Remote-friendly" or "flexible" JDs received no penalty but the ambiguity was noted. (c) "Remote Infrastructure" positive signals were checked: distributed-first culture, async tools mentioned in JD, absence of "collaborative office environment" language.
- **Career gap / returner:** If plan-carrera.md shows a career gap, scoring was not penalized for the gap itself. Seniority Fit was scored based on total pre-gap experience years, not recency. If the JD has explicit "recent experience" language (e.g., "3+ years of recent PM experience"), this was flagged in the Skill Match breakdown as a potential filter risk, not an automatic NONE.
- **Founder-fit dimension modifier (failed founder / shut-down company):** If plan-carrera.md shows founder/CEO/co-founder experience at a company that shut down, failed, or was acqui-hired at low value, add a "Founder-Fit" dimension modifier to the scoring: +5 for companies that explicitly value entrepreneurial experience, -5 for companies with rigid hierarchy signals. Flag any JD language like "thrives in structured environments" or "follows established processes" as potential friction for former founders.
- **Ageism-signal detection (veteran / 15+ years experience):** If plan-carrera.md shows 15+ years of experience, or experience at legacy/enterprise companies (Oracle, IBM, SAP, HP, etc.), or explicit mention of age-related concerns, scan the JD for potential age-bias signals. Red flags: "digital native," "recent graduate preferred," "1-3 years experience" for senior roles, "high-energy environment," "young and dynamic team," "culture fit" without specifics. Yellow flags: "must be familiar with TikTok/Instagram/Snap" (may be legitimate but could signal youth preference). If 3+ red flags are detected, add a WARNING in the output: "POTENTIAL AGE BIAS SIGNALS DETECTED in this JD. Consider whether this company's culture would be welcoming." Do NOT auto-deduct points -- just flag for the user's awareness.
- **Military-to-PM career changer (Security Clearance dimension modifier):** If plan-carrera.md shows military background (active duty, veteran, reserves, or military titles like Captain, Major, Lieutenant, Colonel, etc.), apply these scoring adjustments: (a) If user has active TS/SCI and role is at a defense tech company (Palantir, Anduril, Shield AI, Rebellion Defense, or any company where the JD mentions clearance): +15 bonus to total score. An active TS/SCI clearance is extremely valuable and expensive to obtain ($50K-$150K to sponsor, 6-12 month timeline). This is a MAJOR differentiator. (b) If user has active clearance (any level) and role is at a company that does government work (even if not defense tech): +5 bonus to total score. (c) If role explicitly requires a clearance and user has one: flag as MAJOR advantage in the Recommendation section. (d) TRACK SCORING: Score defense tech roles and general tech roles with different emphasis. Defense tech roles should score significantly higher for military candidates due to clearance value, mission understanding, and end-user familiarity. General tech roles should be scored purely on transferable skills with no military-specific bonus (except clearance value where applicable). (e) In the Domain Valence Indicator: military experience is an ASSET for defense tech, NEUTRAL-to-ASSET for government-adjacent tech, and requires TRANSLATION for general consumer/enterprise tech.
