# Parte 2: Networking - Viernes, 25 de septiembre de 2026

## Gate de Calidad — Contexto Verificado

`empresas-objetivo.md` (última actualización 2026-08-10) y `plan-carrera.md` tienen datos reales, no placeholders. `rastreador-conexiones.md` también tiene datos reales (35 conexiones documentadas, importadas de LinkedIn el 2026-08-13), aunque **no se actualiza hace 43 días**. El briefing continúa con los tres archivos.

**Modo detectado:** MODO REMOTO activo — `plan-carrera.md` marca remoto como filtro duro ("Remoto excluyente"). No aplica MODO DIRECTOR+/EMPLEADO (el usuario no está empleado actualmente — contrato en Amplifire terminó hace ~1 mes). No aplica MODO RETURNER — el gap de ~1 mes es una transición normal entre roles, no un gap de carrera extendido que requiera reactivación de red.

---

## Limitación Estructural — Por Qué No Hay 25 Solicitudes de Conexión Nuevas Hoy

Según el propio diseño de `.claude/skills/solicitud-conexion/SKILL.md`, el sistema **no tiene acceso directo a LinkedIn para buscar personas reales** en empresas con gap de cobertura — requiere que el usuario pegue resultados de búsqueda de LinkedIn (nombre, rol, cualquier post reciente). Esta sesión automatizada no tiene ese input, y por la regla anti-fabricación de `CLAUDE.md` ("NUNCA fabricar experiencia... ni inventar habilidades, proyectos ni métricas"), ese mismo principio aplica a inventar personas: no se van a generar 25 nombres, títulos y "connection points" de contactos que no fueron verificados por el usuario. Hacerlo sería peor que no producir el output — el usuario terminaría enviando solicitudes a perfiles potencialmente inexistentes, desactualizados o mal targeteados.

Un `WebSearch` exploratorio hoy sí encontró perfiles públicos reales indexados (ej. reclutadores de Anthropic y Nubank) — pero son hallazgos de motor de búsqueda sin verificación de vigencia (¿siguen en el rol? ¿el título es actual?), exactamente el tipo de dato que el propio skill excluye a propósito. No se incluyen como solicitudes generadas.

### Qué hacer en su lugar

Pegá los resultados de esta búsqueda en LinkedIn para cada empresa (te doy el prompt exacto, empresas priorizadas para cumplir la regla de MODO REMOTO — al menos 50% del lote a empresas remote-friendly confirmadas):

```
Necesito perfiles de LinkedIn para armar solicitudes de conexión para [Empresa].
Buscá: "[Empresa]" AND ("Product Manager" OR "PM" OR "Engineering Manager" OR "Design Lead" OR "Recruiter")
Necesito 3 personas: 1-2 PMs a mi nivel o un nivel arriba, 1 reclutador/a o rol adyacente.
Para cada persona: nombre, rol actual, y cualquier post reciente o dato compartido (escuela, empresa previa, ciudad).
```

**Distribución sugerida para el próximo lote de 25 (round-robin, ≥50% remote-friendly confirmado):**

| Grupo | Empresas | Cupo sugerido |
|---|---|---|
| Remote-friendly confirmado (100% remoto declarado) | GitLab, Deel, Shopify, Vercel, Figma | 4+4+3+2+2 = 15 |
| Prioridad Tier 1 (gap 0 conexiones, fit fuerte) | Nubank, Stripe (equipo GPTN — remoto LatAm/NA confirmado hoy en `briefings/2026-09-25-part1-roles.md`), VTEX, Anthropic | 3+3+2+2 = 10 |

Empresas excluidas de esta ronda por ya tener ≥4 conexiones: Globant (16), Mercado Libre (16), Microsoft (5). Empresas con gap pero baja prioridad (Amazon 3, Apple 2, Google 2, Salesforce 2, Atlassian 1) tienen conexiones reales existentes — ver reactivación abajo en vez de nuevas solicitudes.

**Networking virtual de esta semana (MODO REMOTO):** Unirte al Slack de Product School y comentar en 2-3 threads relevantes esta semana. También considerar la comunidad de Lenny (Lenny's Newsletter community) — alta concentración de PMs remotos y de empresas del Tier 1 (Stripe, GitLab, Notion, Figma).

---

## Solicitudes de Conexión (0 generadas hoy — ver limitación arriba)

Ninguna solicitud nueva se generó en este briefing automatizado. Pegá los resultados de LinkedIn con el prompt de arriba y corré `/solicitud-conexion` para el lote completo.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

`rastreador-conexiones.md` no registra ninguna solicitud enviada con fecha (todas las 35 conexiones documentadas son de 1er grado ya establecidas desde hace años, importadas del CSV de LinkedIn el 2026-08-13 — no hay entradas de estado "solicitada" con fecha reciente). No hay forma de detectar conexiones que pasaron a "conectada" en las últimas 48 horas porque no hay solicitudes en curso registradas. Ninguna se genera hoy.

**Nota:** una vez que se envíe el primer lote de solicitudes (ver sección anterior), actualizá `rastreador-conexiones.md` con fecha de envío para que esta sección pueda funcionar en briefings futuros.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)
Ninguno. No existe `referral-tracker-template.md` ni ningún registro de pedidos de referido enviados con fecha — no hay nada de qué hacer seguimiento todavía.

### Roles postulados en 48hs sin referido
Ninguno. Según `briefings/2026-09-25-part1-roles.md`, el conteo de postulaciones formalmente registradas sigue en 0 desde el inicio del sistema.

### Nuevos Pedidos de Referido — Los 6 Contactos de Mayor Prioridad

`rastreador-conexiones.md` ya identificó estos 6 contactos como los de mayor prioridad para activar (rol relevante + acceso directo a vacantes/decisiones) y recomendó explícitamente correr `/pedir-referido` para ellos antes de seguir generando CVs. Son consultas iniciales — cálidas, sin pedir referido directo todavía (es el primer touch). Tratamiento ajustado por país; donde no hay país confirmado en el tracker, se usa "tú" y se marca la duda.

**1. Elena Yndurain — Microsoft, Director AI Product Management** [tú — asumiendo España, no confirmado en tracker]
> Hola Elena, vi tu rol liderando AI Product Management en Microsoft y me pareció el mejor punto de contacto para una pregunta puntual. Vengo de liderar el diseño end-to-end de un chatbot de soporte con IA (RAG, LLM, arquitectura de prompts) en una plataforma de adaptive learning, y estoy evaluando mi próximo paso enfocado en producto de IA. ¿Tendrías 15 minutos para contarme cómo ves el mercado de AI PM hoy, y si hay señal de vacantes en tu equipo o en Microsoft en general?

**2. Virginia Silvero — Globant, Regional Recruiter Lead, South of LatAm** [vos — Argentina, coherente con el resto de la red de Globant del usuario]
> Hola Virginia! Vi que liderás recruiting regional en Globant para el sur de LatAm. Tengo 15+ años en Product Management (AI, fintech, salud digital), el último tramo liderando un producto de IA conversacional (RAG/LLM) en una plataforma EdTech. Estoy evaluando mi próximo rol de PM y me encantaría saber si hay vacantes activas o el mejor canal para postular. ¿Tenés 15 minutos esta semana?

**3. Melina Ruggeri — Salesforce, LATAM Recruiting Senior Manager** [vos — asumiendo Argentina por apellido y rol regional, no confirmado]
> Hola Melina! Te contacto porque liderás recruiting LATAM en Salesforce. Tengo 15+ años en Product Management, con foco reciente en productos de IA (chatbot con RAG/LLM en una plataforma EdTech) y antes en fintech/insurtech. Estoy buscando mi próximo rol de PM remoto y quería preguntarte si hay vacantes abiertas en tu radar o el mejor camino para aplicar. ¿Tenés 15 minutos para charlar?

**4. Maria Jose Trejo Conde — Mercado Libre, Regional Talent Acquisition IT Senior Analyst** [tú — país no confirmado en tracker, se usa el default no-Argentina/Uruguay]
> Hola María José, te contacto porque lideras Talent Acquisition IT regional en Mercado Libre. Tengo 15+ años en Product Management (fintech, insurtech, EdTech con IA) y estoy evaluando mi próximo rol de PM remoto en LatAm. ¿Tendrías 15 minutos para comentarme si hay vacantes de producto abiertas o el mejor canal para aplicar?

**5. Bernardo Manzella — Globant, Head of People & Capacity Strategy (AI Studios)** [vos — Argentina, coherente con el resto de la red de Globant del usuario]
> Hola Bernardo! Vi que liderás People & Capacity Strategy para AI Studios en Globant — doble match con mi perfil: PM con foco reciente en productos de IA (lideré un chatbot con RAG/LLM en una plataforma EdTech) y 15+ años en product management. Estoy evaluando mi próximo rol y me encantaría saber si hay vacantes en AI Studios o el mejor canal interno. ¿Tenés 15 minutos?

**6. Pedro Alejandro Santamarina — Mercado Libre, Sr. Product Development Manager** [vos — Argentina, coherente con el resto de la red de MELI del usuario]
> Hola Pedro! Sos el contacto de Product más senior que tengo en Mercado Libre, así que te escribo directo. Vengo de 15+ años liderando producto (fintech, insurtech, EdTech con IA), el último rol liderando un chatbot con IA (RAG/LLM) a escala enterprise. Estoy evaluando mi próximo paso como PM y me encantaría 15 minutos para escuchar cómo ves el equipo de producto en MELI hoy, y si hay una vacante donde pueda calzar.

**Después de enviar estos 6 mensajes:** actualizá `rastreador-conexiones.md` con la fecha de envío de cada uno, para que el briefing de mañana pueda detectar respuestas y generar recordatorios a los 5+ días si hace falta.

---

## Reconexión — Conexiones Existentes en Empresas con Gap (<4 conexiones)

Estas son conexiones reales ya establecidas, no nuevas solicitudes — el próximo paso es reconectar, no pedir. Priorizadas por el tracker:

- **Elena Yndurain** (Microsoft, Director AI Product Management) — cubierta arriba como pedido de referido directo por relevancia altísima.
- **Melina Ruggeri** (Salesforce, LATAM Recruiting Senior Manager) — cubierta arriba.
- **Pablo Perez** (Apple, AIML) — marcado "Prioridad — rol de IA/ML" en el tracker, sin acción tomada aún. Sugerido para el batch de mañana si no hay respuesta de los 6 de arriba.
- **Alejandro Medici** (Amazon/AWS, Startup Solution Architect) — conexión antigua (2013), evaluar reconectar con mensaje de reactivación de red antes de pedir nada.

---

## Resumen del Día

- 0 solicitudes de conexión nuevas generadas (limitación estructural: sin acceso a búsqueda de LinkedIn, ver arriba) — acción pendiente del usuario: pegar resultados de LinkedIn.
- 0 seguimientos de conexiones aceptadas (sin datos de solicitudes en curso en el tracker).
- 6 pedidos de referido iniciales redactados y listos para enviar hoy — usan datos 100% reales del tracker y de `biblioteca-experiencias.md`.
- 0 recordatorios de referido (sin pedidos previos registrados con fecha).
- El cuello de botella de networking sigue siendo el mismo que señalan `rastreador-conexiones.md` (43 días sin actualizar) y el briefing de Parte 1 de hoy: hay acción identificada y lista para ejecutar, pendiente de que el usuario la envíe y registre las fechas.
