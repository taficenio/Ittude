# Parte 2: Networking - Martes, 15 de septiembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: contiene datos reales (2,092 conexiones importadas de LinkedIn, cruzadas contra `empresas-objetivo.md`; última actualización 2026-08-13). ✅ Gate superado.
- `empresas-objetivo.md`: contiene datos reales (108 empresas rankeadas por tier; última actualización 2026-08-10). ✅ Gate superado.
- `plan-carrera.md`: contiene datos reales (nivel, modalidad remoto-excluyente, mercado objetivo, debilidades). ✅ Gate superado.

## Detección de Tipo de Rol y Modo

- **Función objetivo:** Product Manager / Product Owner (IC senior, Lead/Head, o especialización en IA — tres caminos abiertos, sin ranking estricto).
- **Modo Director+/Empleado:** NO aplica. `plan-carrera.md` no indica nivel Director+, y el usuario no está empleado actualmente (contrato en Amplifire terminó hace ~1 mes; está evaluando activamente su próximo rol).
- **Modo Remoto:** SÍ aplica. `plan-carrera.md` marca la modalidad remota como **filtro duro, excluyente** ("Remoto excluyente — no considerar roles híbridos ni presenciales"). Se asignó el lote priorizando empresas remote-friendly confirmadas en `empresas-objetivo.md` (ver desglose abajo).
- **Modo Returner:** NO aplica en el sentido estricto del modo. El gap de empleo actual (~1 mes) ya fue reencuadrado en `plan-carrera.md` como transición normal, no como un gap de carrera que requiera reactivación de red dormida como estrategia central. No se fuerza el bloque de "Reactivación de Red".

## Nota de Método — Fuente de los Prospectos (importante)

`rastreador-conexiones.md` solo tiene nombres reales para las 9 empresas donde el usuario ya tiene conexiones de 1er grado (Globant, Mercado Libre, Microsoft, Amazon, Apple, Google, Salesforce, Atlassian, Naranja X). Para las 99 empresas objetivo sin ninguna conexión, el tracker no lista ningún prospecto — por diseño, ese es exactamente el gap de cobertura.

Regla del sistema: nunca fabricar información. En vez de inventar nombres para completar la tabla, cada persona listada abajo fue encontrada vía `WebSearch` (perfiles públicos de LinkedIn indexados) inmediatamente antes de generar este briefing. Los mensajes usan **solo** lo que aparece en el snippet de búsqueda (nombre, rol, y detalle de su trabajo cuando estaba disponible) como punto de conexión — no se inventó conexión mutua, escuela compartida ni ubicación no confirmada. `WebFetch` sigue bloqueado (ver `briefings/2026-09-15-part1-roles.md`), así que no fue posible abrir el perfil completo de cada persona para verificar más detalle — tratá cada nombre como un candidato a verificar visualmente en LinkedIn antes de enviar la solicitud, no como un dato 100% confirmado.

De las empresas con gap se cubrieron **16 de 99** en esta ronda (las de mayor prioridad Tier 1/2, ponderando remoto). Las 83 restantes (Kavak, Remote.com, y el resto del Tier 2/3/4) quedan pendientes para próximas rondas — para Kavak y Remote.com específicamente, la búsqueda de hoy no devolvió ningún perfil real utilizable (falsos positivos o sin indexación pública), así que se excluyeron de este lote en vez de fabricar un contacto.

---

## Solicitudes de Conexión (25 en total)

**Distribución Modo Remoto:** 13 de 25 (52%) a empresas remote-friendly confirmadas en `empresas-objetivo.md` (GitLab — 100% remota desde su fundación; Deel — infraestructura full-remote; Nubank — remoto regional LatAm; Atlassian, Shopify, Twilio, Vercel, Linear — categoría "SaaS remoto-friendly, contratación LatAm confirmada"). El resto (12) va a otras empresas Tier 1/2 con gap de cobertura, incluyendo Anthropic, Stripe, HubSpot, Notion, Duolingo, Rappi, Bitso y VTEX.

**Tratamiento:** tú por defecto (convención para la mayoría de los países no-Argentina/Uruguay); vos solo donde el snippet confirmó ubicación en Argentina (fila 6, Beatriz Faria).

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Jess (Cummings) Dallmar | GitLab | VP, Global Talent Acquisition | Hola Jess, te escribo porque lideras Talent Acquisition global en GitLab, una de las pocas empresas 100% remote-first desde su fundación. Soy Ramón, PM con 15+ años liderando producto en equipos remotos de LatAm, USA y Nueva Zelanda. Me encantaría sumarte a mi red. |
| 2 | Heather Tarver | GitLab | Sr. Technical Recruiter | Hola Heather, vi tu rol como Sr. Technical Recruiter en GitLab. Soy Ramón, PM senior (15+ años) con foco reciente en IA aplicada a producto. Me interesa mucho la cultura remote-first de GitLab -- me encantaría conectar y conocer cómo evalúan a PMs. |
| 3 | Ben Cowdry | GitLab | Recruitment Manager | Hola Ben, vi tu rol como Recruitment Manager en GitLab. Soy Ramón, PM con 15+ años liderando producto para equipos 100% distribuidos -- justo el modelo de GitLab. Me encantaría sumarte a mi red y entender mejor cómo arman sus equipos de Producto. |
| 4 | Ana Freymuth | Deel | Senior Global Talent Acquisition (Product Leadership) | Hola Ana, vi que llevás Talent Acquisition global en Deel con foco en Product Leadership. Soy Ramón, PM con 15+ años liderando producto para equipos remotos e internacionales -- la misma lógica que Deel resuelve como infraestructura. Me encantaría conectar. |
| 5 | Florencia Gandulia Nordmann | Deel | Talent / LATAM hiring | Hola Florencia, vi tu trabajo en hiring para LatAm en Deel. Soy Ramón, PM argentino con 15+ años liderando producto para empresas globales sin relocalizarme -- exactamente lo que Deel habilita. Me encantaría sumarte a mi red. |
| 6 | Beatriz Faria | Nubank | Talent Acquisition (Argentina) | Hola Beatriz, vos estás en Talent Acquisition de Nubank en Argentina. Soy Ramón, PM con 15+ años en producto fintech/regulado (seguros, pagos, compliance fiscal). Nubank es una de mis empresas objetivo en LatAm -- ¿te sumo a mi red? |
| 7 | Luana Oliveira | Nubank | Talent Operations Analyst / Recruitment Lead | Hola Luana, vi tu rol liderando Recruitment/Talent Ops en Nubank. Soy Ramón, PM con 15+ años en producto fintech (pagos, DeFi, seguros). Nubank es una de las fintechs que más sigo en LatAm -- me encantaría sumarte a mi red. |
| 8 | Ashley Gregory | Atlassian | Technical Recruiter, Product | Hola Ashley, vi que reclutás específicamente para Producto en Atlassian. Soy Ramón, PM con 15+ años de experiencia, incluyendo años de uso profundo de Jira/Confluence del lado cliente. Me encantaría sumarte a mi red y conocer más del equipo de Producto. |
| 9 | Sophia Abadiano | Shopify | Apprentice Product Manager | Hola Sophia, vi tu camino como Apprentice PM en Shopify. Soy Ramón, PM senior con 15+ años liderando producto (eCommerce, fintech, EdTech). Shopify es de las culturas de producto remote-first que más admiro -- me encantaría sumarte a mi red. |
| 10 | Daniela Bohórquez | Twilio | Sr. Manager, Talent Acquisition (GTM/Marketing, Americas) | Hola Daniela, vi que lideras Talent Acquisition GTM para Americas en Twilio. Soy Ramón, PM con 15+ años liderando producto en LatAm y USA sin relocalización. Twilio es una de mis empresas objetivo -- me encantaría sumarte a mi red. |
| 11 | Evan Funk | Vercel | Talent | Hola Evan, vi que estás reclutando activamente para Vercel. Soy Ramón, PM con 15+ años en producto, con foco reciente en IA aplicada (RAG, LLM, arquitectura de prompts) en un producto EdTech. Me encantaría sumarte a mi red y conocer más del equipo. |
| 12 | Joshua Poore | Vercel | Data & AI teams | Hola Joshua, vi que estás armando los equipos de Data & AI en Vercel. Soy Ramón, PM con foco reciente en IA aplicada a producto: definí arquitectura de prompts, RAG y evaluación de modelos en un producto EdTech. Me encantaría sumarte a mi red. |
| 13 | Marlene Guardado | Linear | Recruiting | Hola Marlene, vi que trabajás en Recruiting en Linear junto al equipo de Engineering. Soy Ramón, PM con 15+ años liderando producto, usuario de herramientas ágiles como Linear en varios roles. Me encantaría sumarte a mi red. |
| 14 | Marisa Hurtado | Anthropic | Recruiter (Product Managers) | Hola Marisa, vi que reclutás PMs para Anthropic. Soy Ramón, PM con 15+ años de experiencia y foco reciente en IA aplicada: lideré arquitectura de un chatbot con LLM, RAG y modelos fine-tuneados en un producto EdTech. Me encantaría sumarte a mi red. |
| 15 | Emilie Schwartz | Stripe | Technical Recruiting Lead (payment methods LATAM) | Hola Emilie, vi que tu equipo en Stripe trabaja en payment methods para LatAm. Soy Ramón, PM con experiencia en pagos y reconciliaciones (seguros) y compliance fiscal automatizado. Me encantaría sumarte a mi red y conocer más del equipo. |
| 16 | Amy Salazar | Stripe | Recruiting (0-to-1 builds) | Hola Amy, vi tu foco en recruiting para builds 0-to-1 en Stripe. Soy Ramón, PM con 15+ años liderando producto, incluyendo migraciones y builds desde cero (cloud, IA aplicada). Me encantaría sumarte a mi red y conocer más de Stripe. |
| 17 | Yesenia Reyna | HubSpot | Global Recruiter, LATAM | Hola Yesenia, vi tu rol como recruiter LatAm en HubSpot. Soy Ramón, PM argentino con 15+ años liderando producto para empresas globales de forma remota. HubSpot es una de mis empresas objetivo -- me encantaría sumarte a mi red. |
| 18 | Angela N. | HubSpot | Talent Acquisition Coordinator (LATAM) | Hola Angela, vi que coordinás Talent Acquisition para LatAm en HubSpot. Soy Ramón, PM con 15+ años de experiencia liderando producto en equipos remotos e internacionales. Me encantaría sumarte a mi red y conocer más del proceso. |
| 19 | Dylan Ruane | Notion | Talent | Hola Dylan, vi tu trabajo en Talent en Notion. Soy Ramón, PM con 15+ años liderando producto, usuario habitual de herramientas como Notion en distintos equipos. Me encantaría sumarte a mi red y conocer más del equipo de Producto. |
| 20 | Andy Cipolaro | Duolingo | Sr. Principal Recruiter | Hola Andy, vi tu rol como Sr. Principal Recruiter en Duolingo. Soy Ramón, PM con foco en IA aplicada a EdTech: lideré un chatbot con LLM/RAG para adaptive learning en mi último rol. Duolingo es un match directo con mi especialización. |
| 21 | Renee Davis | Duolingo | Talent Acquisition | Hola Renee, vi tu rol en Talent Acquisition de Duolingo. Soy Ramón, PM con experiencia reciente en IA aplicada a EdTech (adaptive learning, RAG, LLM). Duolingo combina exactamente mi especialización -- me encantaría sumarte a mi red. |
| 22 | Nicolas Esteban Morales Gonzalez | Rappi | Senior Product Manager (Bogotá) | Hola Nicolás, vi tu rol como Senior Product Manager en Rappi. Soy Ramón, PM argentino con 15+ años liderando producto en LatAm y mercados globales. Me encantaría sumarte a mi red y escuchar cómo es el día a día de Producto en Rappi. |
| 23 | Tommy Deane | Bitso | Head of Recruiting | Hola Tommy, vi tu rol liderando Recruiting en Bitso. Soy Ramón, PM con experiencia en fintech/DeFi (coordiné equipos distribuidos en 4 países para un producto cripto). Bitso está en mi radar -- me encantaría sumarte a mi red. |
| 24 | Denis Tobias | Bitso | Product Manager (Brasil) | Hola Denis, vi tu rol como Product Manager en Bitso. Soy Ramón, PM con 15+ años liderando producto, incluyendo un producto cripto/DeFi con equipos distribuidos en 4 países. Me encantaría sumarte a mi red y comparar notas de Producto fintech. |
| 25 | Maíra Sampaio | VTEX | Talent Acquisition / Tech Recruiter | Hola Maíra, vi que estás reclutando para roles de Producto en VTEX. Soy Ramón, PM con 15+ años liderando producto eCommerce/fintech en LatAm y mercados globales. Me encantaría sumarte a mi red y conocer más sobre las posiciones abiertas. |

**Verificación de longitud:** las 25 mensajes fueron medidos programáticamente. El más largo tiene 269 caracteres (fila 1) — todos por debajo del límite de 300 de LinkedIn.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Nada para reportar.** `rastreador-conexiones.md` no tiene una columna de estado ("solicitada" → "conectada") ni fechas de solicitud registradas — solo lista conexiones ya existentes desde la importación original del CSV de LinkedIn (2,092 conexiones, cruzadas el 2026-08-13). No hay forma de detectar si alguna de las ~304+ solicitudes generadas en briefings anteriores fue enviada o aceptada, porque ninguna quedó marcada como enviada (ver nota de Parte 1: "de los ~304+ mensajes de networking ya generados... ninguno está marcado como enviado").

**Acción recomendada (no automatizable):** después de enviar las 25 solicitudes de hoy, actualizar `rastreador-conexiones.md` con fecha de envío por persona. Sin ese dato, este bloque seguirá vacío en cada corrida futura.

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
**Nada para reportar bajo la regla automática.** La regla dispara sobre "roles postulados en las últimas 48 horas sin referido" — y hay 0 postulaciones registradas (confirmado en `briefings/2026-09-15-part1-roles.md`: "Postulaciones enviadas: 0"). Sin una postulación real, no hay una oferta específica para la cual pedir referido.

**Nota aparte (no es un pedido automático, es la recomendación ya señalada por el propio tracker):** `rastreador-conexiones.md` mantiene una lista de 6 conexiones de alta prioridad para activar vía `/pedir-referido` de forma proactiva, sin esperar a una postulación: Elena Yndurain (Microsoft, Director AI Product Management), Virginia Silvero (Globant, Regional Recruiter Lead), Melina Ruggeri (Salesforce, LATAM Recruiting Sr. Manager), Maria Jose Trejo Conde (Mercado Libre, Talent Acquisition IT regional), Bernardo Manzella (Globant, Head of People & Capacity Strategy - AI Studios) y Pedro Alejandro Santamarina (Mercado Libre, Sr. Product Development Manager). Ninguna tiene un pedido enviado según el tracker. Correr `/pedir-referido` manualmente para alguna de estas 6 sigue siendo, según el propio sistema, más eficiente que seguir sumando postulaciones frías.

### Recordatorios (5+ días, sin respuesta)
**Nada para reportar.** `plantillas/template-rastreador-referidos.md` solo tiene placeholders sin completar (`[Nombre]`, `[Título del Rol]`, etc.) — no hay ningún pedido de referido real registrado con fecha de envío, así que no hay nada que cumpla el umbral de 5+ días sin respuesta. Este archivo necesita completarse cada vez que se envíe un pedido real de referido para que este bloque pueda funcionar en corridas futuras.

---

## Resumen de Bloqueos Estructurales (para consistencia con Parte 1)

1. **Sin columna de estado en `rastreador-conexiones.md`:** impide detectar aceptaciones recientes y medir la tasa de conversión de las solicitudes ya generadas.
2. **`template-rastreador-referidos.md` sin completar:** impide automatizar recordatorios de referidos.
3. **`WebFetch` bloqueado (39+ días consecutivos, ver Parte 1):** impidió verificar los 25 perfiles de LinkedIn de hoy más allá del snippet de búsqueda — tratarlos como candidatos a confirmar visualmente antes de enviar cada solicitud, no como datos 100% verificados.
