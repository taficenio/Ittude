# Parte 2: Networking - Miércoles, 7 de octubre de 2026

**Contexto de la corrida:** `git pull origin main` traído al inicio — Parte 1 de hoy (`2026-10-07-part1-roles.md`) ya estaba commiteada, corrida ~15 min antes. Se leyó para contexto de roles top.

**Gate de calidad:** `rastreador-conexiones.md`, `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) — se continúa con output completo.

**Detección de modo (`plan-carrera.md`):** función objetivo = Product Manager/Product Owner. Modalidad remota excluyente confirmada ("filtro duro") → **MODO REMOTO activo**. No es Director+/empleado (sin rol actual — contrato en Amplifire terminó hace ~1 mes) → no aplica modo ejecutivo confidencial. Gap de empleo es de ~1 mes (transición normal, no gap de carrera extendido, según corrección del 2026-08-11 en `plan-carrera.md`) → no se activa MODO RETURNER / reactivación de red dormida.

---

## Solicitudes de Conexión (25 en total)

**Metodología (disciplina anti-fabricación, consistente con las ~18 corridas previas):** este entorno no tiene acceso directo a LinkedIn (ni browser, ni API). Las 25 personas de abajo se identificaron vía `WebSearch` contra fuentes públicas indexadas (perfiles de GitLab.com, Product School, Crunchbase, páginas de speakers de eventos de la propia empresa, Product Hunt) donde nombre + rol + empresa actual eran verificables en el snippet — son personas reales por research dirigido, no contactos confirmados de tu red ni inferencias ni nombres inventados. Se cruzaron contra los ~115 nombres ya usados en las 18 corridas anteriores de Parte 2 (15/09 al 06/10) para evitar duplicados exactos.

**Empresas con gap intentadas sin perfil verificable hoy** (se descartaron en vez de forzar un match débil): Deel y Notion fueron intentadas con múltiples variantes de búsqueda — Deel sí dio 2 nombres verificables (Nicolas Nemni vía Product Hunt, Lisa Wallace vía speakers de "Big Deel 2025 NY"), pero Notion no arrojó ningún PM actual identificable hoy (solo postings de trabajo y comp data). Vercel: ningún nombre verificable hoy, solo job postings.

**Prioridad Deel confirmada:** `empresas-objetivo.md` y el tracker de conexiones marcan a Deel sin ningún contacto de 1er grado, y `2026-10-07-part1-roles.md` identificó un segundo rol ahí hoy (Senior PM FinTech, 80/100) — ya son dos postings de Deel sin ninguna conexión. Se priorizaron los 2 nombres reales encontrados.

**Mezcla remota confirmada (MODO REMOTO):** 25 de 25 (100%) son empresas explícitamente remote-friendly según `empresas-objetivo.md` (Deel y GitLab en Tier 1; Atlassian, Shopify, Twilio, HubSpot, Zendesk, monday.com, Figma, GitHub en el listado SaaS remote-friendly de Tier 2) — muy por encima del mínimo de 50%.

Round-robin: entre 1 y 4 personas por empresa (10 empresas), nunca más de 7. Tratamiento: inglés para todas — ninguna de las 25 personas encontradas hoy pudo confirmarse en país hispanohablante de LatAm vía el snippet de búsqueda.

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Nicolas Nemni | Deel [Tier 1, remote-friendly] | Group Product Manager | Hi Nicolas — Group PM at Deel, the remote-hiring infra that mirrors my own career across Argentina/US/NZ, caught my eye. 15+ yrs PM in fintech/insurtech (payments), now adding AI (MSc, U. Auckland). Would love to connect. |
| 2 | Lisa Wallace | Deel [Tier 1, remote-friendly] | Director of Product, Compensation | Hi Lisa — leading Compensation Product at Deel is sharp territory, close to my own comp/payments background. 15+ yrs PM in fintech/insurtech (payments, reconciliations), now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 3 | Gabe Weaver | GitLab [Tier 1, remote-friendly] | Senior PM, Planning | Hi Gabe — Senior PM on GitLab's Planning solution within the DevOps platform caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland, LLM/RAG shipped in production). Would love to connect. |
| 4 | Jeff Tucker | GitLab [Tier 1, remote-friendly] | Senior PM, Manage: Foundations | 15+ yrs across product, design and eng, now Senior PM for Manage:Foundations at GitLab — that's a track record, Jeff. I have similar tenure in fintech/insurtech, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 5 | Michelle Chen | GitLab [Tier 1, remote-friendly] | Senior Product Manager | Hi Michelle — Senior PM at GitLab, one of the clearest 100%-remote cultures in tech, stood out. I lead distributed teams myself (Argentina/US/NZ), 15+ yrs in fintech/insurtech, now specializing in AI. Would love to connect. |
| 6 | Avinoam Zelenko | Atlassian [remote-friendly] | Principal Product Manager | Hi Avinoam — Principal PM at Atlassian caught my eye. I've used Jira/Confluence client-side for 15+ yrs across telecom/insurtech (UCG, Vortex), now specializing in AI (MSc, U. Auckland). Would love to connect and hear your take. |
| 7 | Matt Tse | Atlassian [remote-friendly] | Senior PM, Enterprise Cloud (Jira/Confluence) | Hi Matt — Senior PM on Enterprise Cloud for Jira/Confluence stood out, deep in tools I've used client-side for 15+ yrs (UCG, Vortex, Xplor). Now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 8 | Daniel Ayele | Atlassian [remote-friendly] | Senior PM, Confluence collaboration | How does the Confluence collaboration team at Atlassian think about AI-assisted docs? I've relied on Confluence client-side for 15+ yrs in telecom/insurtech and I'm now specializing in AI myself. Would love to connect, Daniel. |
| 9 | Gosia Kowalska | Atlassian [remote-friendly] | Senior Group Product Manager | Hi Gosia — Senior Group PM at Atlassian stood out. I'm a PM with 15+ yrs of deep Jira/Confluence use client-side (UCG, Vortex), now specializing in AI (MSc, U. Auckland). Would love to connect and swap notes. |
| 10 | Tim Beyers | Twilio [remote-friendly] | Senior PM, Voice Connectivity & Payment Connectors | Hi Tim — Senior PM on Voice Connectivity & Payment Connectors at Twilio is close to my own payments background (Vortex, reconciliations end-to-end). 15+ yrs PM in fintech/insurtech, now adding AI. Would love to connect. |
| 11 | Tarunpreet Singh | Twilio [remote-friendly] | Senior Product Manager (12 yrs) | 12 yrs across PM, IT consulting and engineering, now Senior PM at Twilio — strong track record, Tarunpreet. I'm a PM with 15+ yrs in fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 12 | Hanhan Wang | Twilio [remote-friendly] | Senior Manager PM, Linked Profiles | Hi Hanhan — leading Linked Profiles as Senior Manager PM at Twilio caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 13 | Connie Liu | Twilio [remote-friendly] | Senior Manager PM, Engage (Experiences Group) | Curious how the Experiences Group for Engage thinks about product depth at Twilio's scale, Connie. I'm a PM with 15+ yrs across fintech/insurtech, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 14 | Dave Strang | Shopify [remote-friendly] | Staff PM, Checkout | Hi Dave — Staff PM leading checkout at Shopify, a platform millions transact through, caught my eye. I owned payments/reconciliations end-to-end at Vortex (100K+ users), now specializing in AI. Would love to connect. |
| 15 | Amol Patil | Shopify [remote-friendly] | Staff PM, Inventory | Hi Amol — Staff PM leading inventory products at Shopify stood out. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland, LLM/RAG shipped in production). Would love to connect. |
| 16 | Ulaize Hernandez | Shopify [remote-friendly] | Product Lead, Inventory management | Hi Ulaize — leading strategy for inventory management tools at Shopify caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect and swap notes. |
| 17 | Bhavin Prajapati | Shopify [remote-friendly] | PM, Cross-border commerce | Hi Bhavin — PM on cross-border commerce at Shopify stood out, close to my own work automating multi-state compliance (Sovos). 15+ yrs PM, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 18 | Anshu Raj | HubSpot [Tier 1, remote-friendly] | Senior Product Manager | Hi Anshu — Senior PM at HubSpot, a company known for genuinely product-led growth, caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 19 | Mike Jaramillo | HubSpot [Tier 1, remote-friendly] | Senior Product Manager | What's HubSpot's take on PLG for AI-native features these days, Mike? I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI myself (MSc, U. Auckland, LLM/RAG shipped in production). Would love to connect. |
| 20 | Jakub Konik | Zendesk [remote-friendly] | Senior PM (Kraków) | Hi Jakub — Senior PM at Zendesk, based in Kraków, caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 21 | Kate Griggs | Zendesk [remote-friendly] | Senior PM (desde 2020) | 5+ yrs as Senior PM at Zendesk is a strong track record, Kate. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland, LLM/RAG shipped in production). Would love to connect. |
| 22 | Ron Kimhi | monday.com [remote-friendly] | PM, monday Sales CRM | Hi Ron — PM on monday Sales CRM caught my eye, sharp space. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect and hear how your team thinks about it. |
| 23 | Avantika Gomes | Figma [remote-friendly] | Group PM, Design Systems/Prototyping/Dev Tools | Hi Avantika — Group PM leading Design Systems, Prototyping & Dev Tools at Figma, with a decade across Pinterest/MS/Google, stood out. I'm a PM with 15+ yrs in fintech/insurtech, now specializing in AI. Would love to connect. |
| 24 | Allison Weins | GitHub [remote-friendly] | Director, Product Management | Hi Allison — Director of Product Management at GitHub caught my eye. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland, LLM/RAG shipped in production). Would love to connect. |
| 25 | Parsa Zand | GitHub [remote-friendly] | Product Manager II (ex-Microsoft PgM) | Your move from Program Manager at Microsoft to PM II at GitHub is a great arc, Parsa. I'm a PM with 15+ yrs across fintech/insurtech/telecom, now specializing in AI (MSc, U. Auckland). Would love to connect. |

Todos los mensajes verificados por debajo de 300 caracteres (rango real: 189-246).

**Networking virtual de esta semana (MODO REMOTO):** sumate a la comunidad de **Lenny** (Lenny's Newsletter community) y comentá en 2-3 threads sobre AI product management o transición a fintech — rotando respecto a la sugerencia de Product School Slack del 2026-10-06, para no repetir siempre la misma comunidad.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

Ninguno. `rastreador-conexiones.md` sigue sin ningún registro de estado "solicitada → conectada" con fecha desde que se importó el CSV de LinkedIn — solo tiene fechas de conexión originales (la más reciente: Sharik Garzón Terán, Mercado Libre, 19 Nov 2025, muy fuera de la ventana de 48hs). El archivo no se actualizó desde 2026-08-13 (55+ días), así que no hay evidencia de ninguna aceptación nueva en las últimas 48 horas, ni de las 25 solicitudes de hoy ni de ninguna corrida previa (no se puede medir sin que el usuario registre los envíos con fecha).

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido

**Acción #1 de hoy, la más urgente del sistema: desbloquear Globant.** `2026-10-07-part1-roles.md` marca el rol de Globant (Product Manager Senior-Level, fit 72/100) como **bloqueado 3 días consecutivos** por falta de confirmación de modalidad (remoto vs. híbrido) — y el mensaje a Virginia Silvero para desbloquearlo ya está redactado desde el 2026-10-02 y sigue sin enviarse:

> **Virginia Silvero** — Regional Recruiter Lead, South of LatAm, Globant (conectados desde 28 Oct 2010):
> "Hola Virginia, ¡tanto tiempo! Nos conectamos hace años en Globant. Soy Product Leader con 15+ años de experiencia (fintech, healthtech, telecom) y acabo de terminar una Maestría en IA en la Universidad de Auckland. Estoy evaluando volver a sumarme a Globant en un rol de Product, y como Regional Recruiter Lead pensé que podrías orientarme sobre el proceso o, si ves fit, ayudarme con un referido. ¿Tenés 15 minutos para charlar esta semana?"

Sin este mensaje, el CV de Globant ya generado y verificado sigue sin poder usarse.

Los otros 5 pedidos de referido de alta prioridad, identificados en `rastreador-conexiones.md` (sección "Gap de Cobertura") y redactados en corridas previas (2026-10-02), tampoco tienen evidencia de envío registrada — 55+ días sin actualización real del tracker:

- **Elena Yndurain** (Microsoft, Director AI Product Management) — match más directo con tu especialización en IA.
- **Melina Ruggeri** (Salesforce, LATAM Recruiting Senior Manager).
- **Pedro Alejandro Santamarina** (Mercado Libre, Sr. Product Development Manager) — el contacto de Product más senior en tu red actual.
- **Bernardo Manzella** (Globant, Head of People & Capacity Strategy, AI Studios) — doble relevancia (People + IA).
- **Maria Jose Trejo Conde** (Mercado Libre, Regional Talent Acquisition IT Senior Analyst).

(Textos completos de estos 5 mensajes en `briefings/2026-10-02-part2-networking.md`, sección de pedidos de referido — no se reescriben aquí para no generar versiones inconsistentes del mismo pedido.)

### Recordatorios (5+ días, sin respuesta)

Ninguno. No existe `referral-tracker-template.md` en el repo, y `rastreador-conexiones.md` no registra fecha de envío de ningún pedido de referido — sin fecha de envío, no hay nada de qué hacer seguimiento. Los 6 pedidos de arriba están en estado "redactado, nunca confirmado como enviado", no "enviado sin respuesta" — son acción nueva, no recordatorio.

### Roles postulados en las últimas 48 horas sin referido

Ninguno. Según `2026-10-07-part1-roles.md`: 0 postulaciones formales registradas (Postulaciones: 0 | Entrevistas: 0 | Ofertas: 0), pese a 4 CVs ya generados y verificados esperando envío (VTEX desde 2026-09-03 — 34 días de demora, Globant, Deel Staff PM del 2026-10-04, Deel Senior PM FinTech de hoy). El cuello de botella del sistema es 100% de envío humano, no de generación — no hay postulaciones recientes que necesiten un referido de respaldo porque no hay postulaciones.

---

## Resumen de Acción

1. **Enviá el mensaje a Virginia Silvero (arriba)** — es el bloqueador de mayor apalancamiento del sistema hoy: desbloquea el CV de Globant que lleva 3 días consecutivos esperando confirmación de modalidad.
2. **Enviá las 25 solicitudes de conexión nuevas**, distribuidas round-robin entre 10 empresas remote-friendly (Deel, GitLab, Atlassian, Twilio, Shopify, HubSpot, Zendesk, monday.com, Figma, GitHub) — 100% remote-friendly, muy por encima del mínimo de MODO REMOTO.
3. **Activá los otros 5 pedidos de referido de alta prioridad** ya redactados (Elena Yndurain, Melina Ruggeri, Pedro Alejandro Santamarina, Bernardo Manzella, Maria Jose Trejo Conde) — conversión esperada mayor que cualquier solicitud fría nueva, porque son contactos de primer grado confirmados en tu red real.
4. **Sumate a la comunidad de Lenny** esta semana y comentá en 2-3 threads relevantes sobre AI/fintech PM.
5. **Actualizá `rastreador-conexiones.md`** con cualquier solicitud o pedido de referido que efectivamente se envíe, con fecha — el archivo sigue sin una actualización real desde 2026-08-13 (55+ días), lo que impide que este skill detecte aceptaciones o pedidos pendientes reales en corridas futuras. Esto es lo mismo que señaló la Parte 1 de hoy y cada corrida de Parte 2 desde el 15/09.
