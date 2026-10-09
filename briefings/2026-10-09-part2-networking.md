# Parte 2: Networking - Viernes, 9 de Octubre de 2026

**Contexto de la corrida:** `git pull origin main` traído al inicio -- se fusionaron 11 commits remotos (incluida la Parte 1 de hoy, `2026-10-09-part1-roles.md`, corrida ~15 min antes) que esta copia local no tenía. Se leyó para contexto de roles top.

**Gate de calidad:** `rastreador-conexiones.md`, `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) -- se continúa con output completo.

**Detección de modo (`plan-carrera.md`):** función objetivo = Product Manager/Product Owner. Modalidad remota excluyente confirmada ("filtro duro") -> **MODO REMOTO activo**. No es Director+/empleado (sin rol actual -- el contrato en Amplifire terminó hace ~1 mes) -> no aplica modo ejecutivo confidencial. Gap de empleo de ~1 mes (transición normal) -> no se activa MODO RETURNER / reactivación de red dormida.

---

## Solicitudes de Conexión (7 en total -- lote reducido, ver nota de método)

**Nota de método y honestidad (consistente con la disciplina anti-fabricación de las corridas previas):** este entorno no tiene acceso a LinkedIn ni browser -- cada persona abajo se identificó vía `WebSearch` contra fuentes públicas indexadas (perfiles de LinkedIn country-domain, handbook oficial de empresa, bio de speaker en evento, autoría de blog corporativo) inmediatamente antes de generar este briefing, usando **solo** lo que aparece en el snippet verificado como punto de conexión. Nada fue inventado.

**Empresas con gap de cobertura intentadas hoy (18 búsquedas dirigidas):** Vercel, PagerDuty, ServiceNow, Linear, Rippling, Siigo, Automattic, Zapier, PostHog, Grammarly (remote-friendly / SaaS), Rappi, Bitso, Ualá, Habi, NotCo, Stone Co, iFood (LatAm). De estas, **10 no rindieron ningún perfil individual utilizable** (solo job postings de agregadores o páginas de carrera) -- se descartan por hoy sin forzar un match débil: Vercel, PagerDuty, ServiceNow, Linear, Rippling, Siigo, Automattic, Zapier, Grammarly, Bitso, Habi. **PostHog** rindió nombres reales vía su handbook oficial (Anna Szell, Annika Schmid, Cory Slater, Abe Basu, Mike Warren) pero sin ningún dato específico verificable sobre el trabajo de cada uno -- no pasa la barra de "punto de conexión real, no genérico" del skill, así que se descarta también.

**Sesgo geográfico del resultado de hoy:** las únicas 5 empresas con prospectos verificables fueron LatAm (Rappi, Ualá, NotCo, Stone Co, iFood), ninguna de las cuales está marcada explícitamente "remote-friendly" en `empresas-objetivo.md` (a diferencia de GitLab, Deel, Atlassian, etc. ya targeteadas en corridas previas). **Esto significa que el lote de hoy no cumple el umbral de 50% remote-friendly que exige MODO REMOTO** -- no se fuerza el cumplimiento inventando o inflando la etiqueta; se señala el gap con honestidad. Las 5 empresas sí caen dentro del mercado objetivo LatAm confirmado en `plan-carrera.md`, y el user ya tiene track record remoto demostrado (NZ/US) que puede mencionarse en conversación de seguimiento aunque no sea el punto de conexión inicial.

**Tratamiento:** vos para Argentina (Ualá), tú para Chile (Rappi, NotCo), inglés para Brasil (Stone Co, iFood -- no se asume fluidez en portugués del usuario; LinkedIn profesional en Brasil tech acepta inglés ampliamente).

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Pablo de Solminihac | Rappi [Tier 2, LatAm] | Senior Digital Product Manager (Payments) | Hola Pablo — vi que armaste workflows de PM con Claude + MCP (Jira, Notion, Figma) en los squads de wallet/pagos de Rappi. Tengo 15+ años en fintech/insurtech (pagos, reconciliaciones en Vortex), ahora especializándome en IA (Maestría, U. Auckland). ¿Conectamos? |
| 2 | Nicolás Albani | Ualá [Tier 2, LatAm] | Director de Engineering, vertical Créditos | Hola Nicolás — tu rol liderando el vertical de Créditos como Director de Engineering en Ualá me llamó la atención, fintech de crédito creciendo fuerte en Argentina. Soy PM con 15+ años en fintech/insurtech, ahora especializándome en IA (Maestría, U. Auckland). ¿Conectamos? |
| 3 | Carlos Vilches | NotCo [Tier 2, LatAm+IA] | Head of Product Management | Hola Carlos — liderar Product Management en NotCo con 10+ años en tech (retail y SaaS) me llamó la atención — foodtech + IA es una combinación poco común. Soy PM con 15+ años en fintech/insurtech, ahora especializándome en IA (Maestría, U. Auckland). ¿Conectamos? |
| 4 | João Barra | Stone Co [Tier 2, LatAm] | Specialist Product Manager, Investment Platform | Hi João — your work as Specialist Product Manager on Stone's investment platform in São Paulo caught my eye. I'm a PM with 15+ yrs across fintech/insurtech (payments, reconciliations at Vortex), now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 5 | Yule Silvino | Stone Co [Tier 2, LatAm] | Senior Product Manager, Contact Center Platform | Hi Yule — leading squads that improve StoneCo's contact center platform and experience as Senior PM stood out. I'm a PM with 15+ yrs across fintech/insurtech (payments, reconciliations), now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 6 | Alberto Brant (Ottis) | iFood [Tier 2, LatAm] | Product Manager IV (ex-Advolve) | Hi Alberto — your path to Product Manager IV at iFood through the Advolve acquisition stood out. I'm a PM with 15+ yrs across fintech/insurtech (payments, reconciliations at Vortex), now specializing in AI (MSc, U. Auckland). Would love to connect. |
| 7 | Barbara Gomes | iFood [Tier 2, LatAm] | Group Product Manager | Hi Barbara — your work as Group Product Manager at iFood, featured on Amplitude's blog, caught my eye. I'm a PM with 15+ yrs across fintech/insurtech (payments, reconciliations), now specializing in AI (MSc, U. Auckland). Would love to connect. |

Caracteres verificados (conteo explícito, no estimado): #1 = 262/300, #2 = 273/300, #3 = 263/300, #4 = 260/300, #5 = 252/300, #6 = 248/300, #7 = 244/300. Todas con margen de seguridad (≥27 caracteres libres).

**Networking virtual de esta semana (MODO REMOTO):** sumate a **ADPList** o un canal de **Lenny's Newsletter community** y comentá en 2-3 threads sobre transición a PM especializado en IA -- rotando respecto a Product School Slack (usado el 2026-10-08) y la comunidad de Lenny (usada el 2026-10-07).

**Recomendación concreta para mañana:** si el acceso de red mejora, priorizar las 10 empresas remote-friendly que no rindieron hoy (Vercel, PagerDuty, ServiceNow, Linear, Rippling, Automattic, Zapier, Grammarly, más las de días previos ya saturadas) para recuperar el balance de 50% exigido por MODO REMOTO. Alternativa inmediata: pegar manualmente 5-10 resultados de un LinkedIn People Search (ver template del skill `/solicitud-conexion`) para esas empresas específicas.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

Ninguno. `rastreador-conexiones.md` sigue sin ningún registro de transición de estado "solicitada -> conectada" -- solo tiene las fechas de conexión originales de la importación del CSV de LinkedIn (2,092 conexiones, cruzadas 2026-08-13). La fecha más reciente de cualquier conexión es 19 Nov 2025 (Sharik Garzón Terán, Mercado Libre) y 17 Feb 2026 (OGHENETEJIRI Atebefia, Amazon) -- ambas muy fuera de la ventana de 48hs contada desde hoy (9 de octubre de 2026). El archivo sigue sin actualizarse desde 2026-08-13 (**57 días**, coincide con la nota de `2026-10-09-part1-roles.md`), así que no hay forma de medir aceptaciones nuevas de ninguna de las solicitudes sugeridas en corridas previas sin que el usuario registre manualmente los envíos y respuestas.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido

Ninguno generado por el gate formal de esta sección -- el trigger es "roles postulados en las últimas 48 horas sin referido", y `2026-10-09-part1-roles.md` confirma **0 postulaciones formales** registradas en todo el sistema (61 días de búsqueda, pipeline en 0/0/0). No hay ninguna postulación de las últimas 48hs para la cual pedir un referido.

**Nota importante (fuera del trigger formal, pero de mayor apalancamiento que cualquier solicitud nueva):** las mismas 6 conexiones de 1er grado de alta prioridad siguen sin ningún pedido de referido enviado, y 2 acciones puntuales del briefing de hoy siguen pendientes:
1. **Elena Yndurain** (Microsoft) -- Director AI Product Management, el match más directo con la especialización en IA. Sigue siendo la conexión prioritaria sin usar que `2026-10-09-part1-roles.md` marcó como acción #3 de hoy.
2. **Virginia Silvero** (Globant) -- Regional Recruiter Lead, South of LatAm. El mensaje para desbloquear el CV de Globant (36 días de demora) sigue sin enviarse -- marcado como acción #2 en el briefing de hoy.
3. Melina Ruggeri (Salesforce) -- LATAM Recruiting Senior Manager.
4. Maria Jose Trejo Conde (Mercado Libre) -- Regional Talent Acquisition IT Senior Analyst.
5. Bernardo Manzella (Globant) -- Head of People & Capacity Strategy (AI Studios).
6. Pedro Alejandro Santamarina (Mercado Libre) -- Sr. Product Development Manager.

Estos no entran en "Nuevos Pedidos de Referido" porque esa sección depende del gate de postulación de 48hs, no de gaps de referido en general -- pero siguen siendo la acción de mayor conversión disponible hoy. Correr `/pedir-referido` para Virginia Silvero (Globant) desbloquea directamente uno de los 4 CVs ya generados y esperando envío.

### Recordatorios (5+ días, sin respuesta)

Ninguno. `rastreador-conexiones.md` no tiene registrado ningún pedido de referido como enviado (0 de 0), y no existe `referral-tracker-template.md` en el repo. Sin un registro de envíos con fecha, no hay nada que recordar todavía. Esto se repite desde el 2026-08-13: hasta que el usuario actualice el tracker con fechas reales de envío, esta sección seguirá vacía en cada corrida futura, sin importar cuántos pedidos de referido se hayan sugerido.

---

## Resumen de Acción para Hoy

1. Enviar las 7 solicitudes de conexión verificadas (Rappi, Ualá, NotCo, Stone Co x2, iFood x2).
2. Enviar el mensaje a Virginia Silvero (Globant) -- desbloquea el CV de Globant, que sigue sin enviarse.
3. Correr `/pedir-referido` para Elena Yndurain (Microsoft) -- match directo con la especialización en IA.
4. Actualizar `rastreador-conexiones.md` con cualquier envío de hoy -- sin esto, "Seguimientos" y "Recordatorios" seguirán vacíos indefinidamente, no porque no haya actividad sino porque no se está registrando (57 días sin actualización real).
