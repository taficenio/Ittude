# Parte 2: Networking - Miércoles, 14 de Octubre de 2026

**Contexto de la corrida:** `git pull origin main` traído al inicio — sin cambios nuevos que no tuviera ya esta copia (trajo 2 commits que ya estaban reflejados). Parte 1 de hoy (`2026-10-14-part1-roles.md`) ya estaba commiteada (corrida ~15 min antes); se leyó para contexto de roles top.

**Gate de calidad:** `rastreador-conexiones.md`, `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) — se continúa con output completo.

**Detección de modo (`plan-carrera.md`):** función objetivo = Product Manager/Product Owner. Modalidad remota excluyente confirmada ("filtro duro") → **MODO REMOTO activo**. No es Director+/empleado (sin rol actual — contrato en Amplifire terminó hace ~1 mes) → no aplica modo ejecutivo confidencial. Gap de empleo de ~1 mes (transición normal, no gap de carrera extendido) → no se activa MODO RETURNER / reactivación de red dormida.

---

## Solicitudes de Conexión (3 en total — lote reducido, ver nota de método)

**Nota de método y honestidad (consistente con la disciplina anti-fabricación de las ~24 corridas previas):** este entorno no tiene acceso a LinkedIn ni browser — cada persona se identifica vía `WebSearch` contra fuentes públicas indexadas (perfiles LinkedIn country-domain) inmediatamente antes de generar este briefing, usando **solo** lo que aparece en el snippet verificado como punto de conexión. Nada fue inventado.

**Se corrieron 15 búsquedas dirigidas contra 12 empresas con gap de cobertura real** (0 conexiones en `rastreador-conexiones.md`, priorizando remote-friendly para MODO REMOTO y empresas Tier 1 sin intentar antes): Anthropic, Figma, GitHub, Zendesk, Conekta, Satellogic, Perplexity, Asana, Deel, Dropbox, GitLab, Nubank. **Las 12 no rindieron ningún perfil individual utilizable** — mismo patrón ya documentado en corridas previas (2026-10-08, -09, -12, -13): el motor devuelve agregadores de empleo (BuiltIn, Greenhouse, WeLoveProduct, Working Nomads) o el mismo pool reducido de perfiles argentinos genéricos (Daniela Mandl, Gabriel Jurado, Cinthia Varas) que ya aparecieron sin relación real a la empresa buscada en corridas anteriores — se descartan de nuevo por la misma razón. Un resultado de Zendesk (Jhoan Zabala, Chile) se descartó explícitamente: su título menciona "Zendesk Admin" como herramienta, pero su empleador real es Millicom, no Zendesk — no pasa la barra de "empleado verificable de la empresa objetivo".

**3 búsquedas adicionales sobre empresas Tier 2/3 ya con intentos previos fallidos (Cornershop/Uber, Rappi) rindieron 3 personas verificables hoy**, vía perfiles LinkedIn country-domain (cl.linkedin.com, pe.linkedin.com) con rol y proyecto específico confirmados en el snippet:

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Carolina Imarai | Cornershop by Uber [Tier 3, LatAm] | Product Manager — lideró la migración de la app de shoppers de Cornershop a Uber (3 squads: Android, iOS, Web) | Hola Carolina — tu liderazgo migrando la app de shoppers de Cornershop a Uber (3 squads: Android, iOS, Web) me llamó la atención. Soy PM con 15+ años en fintech/insurtech, ahora sumando especialización en IA (Maestría, U. Auckland). ¿Conectamos? |
| 2 | Jorge Cabané | Cornershop by Uber → Uber [Tier 3, LatAm] | Product Owner en Cornershop (Stores Center, Picking & Delivery) → Product Manager, pricing grocery LATAM en Uber | Hola Jorge — tu paso de Product Owner en Cornershop (Stores Center, Picking & Delivery) a liderar pricing de la vertical grocery de Uber en LatAm me llamó la atención. Soy PM con 15+ años en fintech/insurtech, sumando IA (Maestría, U. Auckland). ¿Conectamos? |
| 3 | César Hoshi | Rappi [Tier 2, LatAm] | Product Manager — primer año en el rol, lideró el rediseño de la Restaurant App | Hola César — tu primer año como Product Manager en Rappi liderando el rediseño de la Restaurant App me llamó la atención. Soy PM con 15+ años en fintech/insurtech (pagos, reconciliaciones en Vortex), sumando IA (Maestría, U. Auckland). ¿Conectamos? |

Caracteres verificados (conteo explícito vía herramienta, no estimado): #1 = 253/300, #2 = 265/300, #3 = 258/300. Todos con margen de seguridad (≥35 caracteres libres). Tratamiento: tú (Chile y Perú), según convención LATAM del sistema.

**Nota sobre un hallazgo descartado:** una búsqueda sobre Rappi devolvió un resultado cuya URL (`co.linkedin.com/in/andreslemus`) no coincidía con el nombre citado en el título del snippet ("Daniela Urrea, Product Lead de financiamiento") — la propia herramienta de búsqueda marcó la discrepancia. Se descarta sin usar: un desajuste URL/nombre es exactamente el tipo de dato no verificable que la regla "NUNCA fabricar" de `CLAUDE.md` exige descartar, aplicada a identidad, no solo a experiencia.

**Nota sobre cumplimiento de MODO REMOTO:** no se cumple el umbral de 50%. Las 3 personas de hoy son de Cornershop/Uber y Rappi, ninguna marcada "remote-friendly" en `empresas-objetivo.md` (son operaciones de delivery/gig economy con estructura regional, no remote-first declarado) — a diferencia de GitLab, Deel, Atlassian, etc., que sí lo están pero que otra vez no rindieron ningún prospecto verificable hoy (ver lista de intentos fallidos arriba). No se fuerza el cumplimiento inflando la etiqueta; se señala el gap con honestidad, consistente con el tratamiento de corridas de bajo rendimiento anteriores (2026-10-09, 2026-10-12).

**Empresas con gap que quedaron sin ningún prospecto verificable hoy:** Anthropic, Figma, GitHub, Zendesk, Conekta, Satellogic, Perplexity, Asana, Deel, Dropbox, GitLab, Nubank. (Se suman a la lista ya acumulada de intentos fallidos en corridas previas: Stripe[hit previo], Atlassian, HubSpot, Notion, Duolingo, VTEX, Kavak, Shopify, Twilio, Monday.com, Buffer, Doist, Wise, Adyen, Plaid, MongoDB, PayPal, Scale AI, HashiCorp, Grafana Labs, Fivetran, Creditas, Addi, Lemon Cash, Automattic, Buk, Zapier, Remote.com, Block/Square, Vercel, PagerDuty, ServiceNow, Linear, Rippling, Siigo, PostHog, Grammarly, Bitso, Habi, Brex, Snowflake, Intercom.)

**Recomendación concreta para la próxima corrida:** el patrón estructural ya señalado en 2026-10-13 sigue sin resolverse — `WebSearch` encuentra personas reales de forma confiable solo en empresas LatAm de operación local (delivery, fintech regional: Rappi, Ualá, NotCo, Stone Co, iFood, Betterfly, Cornershop/Uber), no en las empresas Tier 1 remote-first globales (GitLab, Deel, Stripe, Notion, Anthropic) que más importan para MODO REMOTO. Si el acceso de red no mejora, la alternativa de mayor apalancamiento sigue siendo que el usuario pegue manualmente 10-15 resultados de un LinkedIn People Search (ver template del skill `/solicitud-conexion`) para 2-3 empresas Tier 1 remote-first prioritarias (GitLab, Deel, Nubank) — desbloquearía de una vez el déficit de MODO REMOTO que se repite desde el 2026-10-09.

**Networking virtual de esta semana (MODO REMOTO):** sumate a **ADPList** y comentá en 2-3 threads sobre transición a fintech/AI PM — rotando respecto al Slack de Product School (2026-10-12) y la comunidad de Lenny (2026-10-09, 2026-10-13), para no repetir siempre el mismo canal.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

Ninguno. `rastreador-conexiones.md` sigue sin ningún registro de transición de estado "solicitada → conectada" — solo tiene las fechas de conexión originales de la importación del CSV de LinkedIn (2,092 conexiones, cruzadas 2026-08-13). La fecha más reciente de cualquier conexión es 19 Nov 2025 (Sharik Garzón Terán, Mercado Libre) y 17 Feb 2026 (OGHENETEJIRI Atebefia, Amazon), ambas muy fuera de la ventana de 48hs contada desde hoy. El archivo no se actualizó desde 2026-08-13 — **62 días exactos**, coincidiendo con la nota de `2026-10-14-part1-roles.md` sobre el mismo tracker — así que no hay forma de medir aceptaciones nuevas de ninguna solicitud sugerida en corridas previas sin que el usuario registre manualmente los envíos y respuestas.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido

Ninguno generado por el gate formal de esta sección — el trigger es "roles postulados en las últimas 48 horas sin referido", y `2026-10-14-part1-roles.md` confirma **0 postulaciones formales** registradas en todo el sistema (66 días de búsqueda, pipeline en 0/0/0, duodécimo día consecutivo sin un rol nuevo verificable). No hay ninguna postulación de las últimas 48hs para la cual pedir un referido.

**Nota importante (fuera del trigger formal, pero de mayor apalancamiento que cualquier solicitud nueva de hoy):** las mismas 6 conexiones de 1er grado de alta prioridad siguen sin ningún pedido de referido confirmado como enviado — sin cambios respecto a las corridas de los últimos 12+ días:
1. **Elena Yndurain** (Microsoft) — Director AI Product Management, match más directo con la especialización en IA.
2. **Virginia Silvero** (Globant) — Regional Recruiter Lead, South of LatAm. El mensaje que desbloquea el CV de Globant (41 días de demora según `2026-10-14-part1-roles.md`) sigue redactado y sin enviar — el mismo bloqueador señalado en el briefing de hoy.
3. Melina Ruggeri (Salesforce) — LATAM Recruiting Senior Manager.
4. Maria Jose Trejo Conde (Mercado Libre) — Regional Talent Acquisition IT Senior Analyst.
5. Bernardo Manzella (Globant) — Head of People & Capacity Strategy (AI Studios).
6. Pedro Alejandro Santamarina (Mercado Libre) — Sr. Product Development Manager.

(Textos completos de estos 6 mensajes en corridas previas de Parte 2 — no se reescriben aquí para no generar versiones inconsistentes del mismo pedido.)

### Recordatorios (5+ días, sin respuesta)

Ninguno. No existe `referral-tracker-template.md` en el repo, y `rastreador-conexiones.md` no registra fecha de envío de ningún pedido de referido — sin fecha de envío, no hay nada de qué hacer seguimiento. Esto se repite desde el 2026-08-13: hasta que el usuario actualice el tracker con fechas reales de envío, esta sección seguirá vacía en cada corrida futura, sin importar cuántos pedidos de referido se hayan sugerido.

---

## Resumen de Acción para Hoy

1. **Enviá las 3 solicitudes de conexión verificadas** (Carolina Imarai y Jorge Cabané en Cornershop/Uber, César Hoshi en Rappi) — lote chico pero verificado punto por punto.
2. **Enviá el mensaje a Virginia Silvero (Globant)** — sigue siendo el bloqueador de mayor apalancamiento del sistema: desbloquea el CV de Globant, 41 días esperando.
3. **Correá `/pedir-referido` para Elena Yndurain (Microsoft)** — match directo con tu especialización en IA, sin ningún pedido enviado todavía en 12+ corridas.
4. **Si tenés 10 minutos:** pegá manualmente resultados de un LinkedIn People Search para GitLab, Deel o Nubank (ver `/solicitud-conexion`) — son las empresas remote-first de Tier 1 que más necesitás para cumplir MODO REMOTO, y el buscador automático no rindió ningún prospecto ahí hoy ni en corridas anteriores.
5. **Actualizá `rastreador-conexiones.md`** con cualquier envío de hoy o de días previos — 62 días sin una actualización real, lo que impide que este skill detecte aceptaciones o pedidos pendientes reales en corridas futuras.
6. **Sumate a ADPList** y comentá en 2-3 threads relevantes esta semana (MODO REMOTO).
