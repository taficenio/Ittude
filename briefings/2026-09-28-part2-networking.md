# Parte 2: Networking - Lunes, 28 de septiembre de 2026

## Gate de Calidad — Contexto Verificado

`empresas-objetivo.md` (última actualización 2026-08-10, sin cambios desde entonces — 49 días) y `plan-carrera.md` tienen datos reales, no placeholders. `rastreador-conexiones.md` también tiene datos reales (35 conexiones documentadas, importadas de LinkedIn el 2026-08-13), pero **no se actualiza hace 46 días** — ni una sola solicitud, respuesta o reconexión registrada desde entonces. El briefing continúa con los tres archivos.

**Modo detectado:** MODO REMOTO activo — `plan-carrera.md` marca remoto como filtro duro ("Remoto excluyente"). No aplica MODO DIRECTOR+/EMPLEADO (el usuario no está empleado actualmente — contrato en Amplifire terminó hace ~1 mes según `plan-carrera.md`). No aplica MODO RETURNER — el gap de ~1 mes es una transición normal entre roles, no un gap de carrera extendido que requiera reactivación de red.

---

## Nuevas Solicitudes de Conexión — Limitación Estructural (0 generadas hoy)

Por diseño, `.claude/skills/solicitud-conexion/SKILL.md` requiere que el usuario pegue resultados reales de búsqueda de LinkedIn (nombre, rol, dato específico) para cada empresa con gap de cobertura — este sistema no tiene acceso directo a LinkedIn. Esta sesión corre desatendida, sin ese input. Por la regla anti-fabricación de `CLAUDE.md` ("NUNCA fabricar experiencia... ni inventar habilidades, proyectos ni métricas"), el mismo principio aplica a inventar personas: no se generan 25 nombres, títulos ni "connection points" de contactos no verificados. Esta misma limitación se documentó en los briefings de Parte 2 del 15/09, 16/09, 21/09, 22/09 y 25/09 — van 5 sesiones seguidas señalándola sin que se haya resuelto.

### Qué pegar para desbloquear el próximo lote

```
Necesito perfiles de LinkedIn para armar solicitudes de conexión para [Empresa].
Buscá: "[Empresa]" AND ("Product Manager" OR "PM" OR "Engineering Manager" OR "Design Lead" OR "Recruiter")
Necesito 3 personas: 1-2 PMs a mi nivel o un nivel arriba, 1 reclutador/a o rol adyacente.
Para cada persona: nombre, rol actual, y cualquier post reciente o dato compartido (escuela, empresa previa, ciudad).
```

**Distribución sugerida para el próximo lote de 25 (round-robin, ≥50% remote-friendly confirmado por MODO REMOTO):**

| Grupo | Empresas | Cupo sugerido |
|---|---|---|
| Remote-friendly confirmado (declarado 100%/remote-first en `empresas-objetivo.md`) | GitLab, Deel, Shopify, Remote.com, Vercel | 4+4+3+2+2 = 15 |
| Prioridad Tier 1 (gap de 0 conexiones, fit fuerte, sin descartar por modalidad) | Stripe (equipo GPTN/LATAM — modalidad remota LatAm/NA más limpia del sistema según `briefings/2026-09-28-part1-roles.md`), Nubank, VTEX, Anthropic | 3+3+2+2 = 10 |

Empresas excluidas de esta ronda por ya tener ≥4 conexiones reales: Globant (16), Mercado Libre (16), Microsoft (5). Empresas con gap pero conexiones reales ya existentes (Amazon 3, Apple 2, Google 2, Salesforce 2, Atlassian 1) van a reconexión, no a solicitud nueva — ver abajo.

**Networking virtual de esta semana (MODO REMOTO):** Unirte al Slack de Product School y comentar en 2-3 threads relevantes. También considerar la comunidad de Lenny (Lenny's Newsletter community) — alta concentración de PMs remotos y de empresas del Tier 1 (Stripe, GitLab, Notion, Figma).

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

Ninguno. `rastreador-conexiones.md` no tiene ninguna entrada con estado "solicitada" y fecha — las 35 conexiones documentadas son todas de 1er grado ya establecidas desde hace años (importadas del CSV el 2026-08-13). Sin solicitudes en curso, no hay nada que pueda haber pasado a "conectada" en las últimas 48hs.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)
Ninguno. No existe `referral-tracker-template.md` ni ningún pedido de referido registrado con fecha de envío en el repo — no hay nada de qué hacer seguimiento todavía.

### Roles postulados en 48hs sin referido
Ninguno. Según `briefings/2026-09-28-part1-roles.md`, postulaciones formalmente registradas: 0 desde el inicio del sistema (día 50).

### Nuevos Pedidos de Referido — Los 6 Contactos de Mayor Prioridad (sin cambios: van 4 briefings de Parte 2 recomendándolos sin registro de envío)

`rastreador-conexiones.md` identificó estos 6 contactos como los de mayor prioridad para activar (rol relevante + acceso directo a vacantes/decisiones) y recomendó correr `/pedir-referido` para ellos antes de seguir generando CVs. Son consultas iniciales — cálidas, primer touch, sin pedir referido directo todavía. Tratamiento por país donde el tracker lo sugiere; donde no está confirmado, se usa "tú" con nota de duda.

**1. Elena Yndurain — Microsoft, Director AI Product Management** [tú — país no confirmado en tracker]
> Hola Elena, vi tu rol liderando AI Product Management en Microsoft y me pareció el mejor punto de contacto para una pregunta puntual. Vengo de liderar el diseño end-to-end de un chatbot de soporte con IA (RAG, LLM, arquitectura de prompts) en una plataforma de adaptive learning, y estoy evaluando mi próximo paso enfocado en producto de IA. ¿Tendrías 15 minutos para contarme cómo ves el mercado de AI PM hoy, y si hay señal de vacantes en tu equipo o en Microsoft en general?

**2. Virginia Silvero — Globant, Regional Recruiter Lead, South of LatAm** [vos — Argentina]
> Hola Virginia! Vi que liderás recruiting regional en Globant para el sur de LatAm. Tengo 15+ años en Product Management (AI, fintech, salud digital), el último tramo liderando un producto de IA conversacional (RAG/LLM) en una plataforma EdTech. Estoy evaluando mi próximo rol de PM y me encantaría saber si hay vacantes activas o el mejor canal para postular. ¿Tenés 15 minutos esta semana?

**3. Melina Ruggeri — Salesforce, LATAM Recruiting Senior Manager** [vos — asumiendo Argentina por apellido y rol regional, no confirmado]
> Hola Melina! Te contacto porque liderás recruiting LATAM en Salesforce. Tengo 15+ años en Product Management, con foco reciente en productos de IA (chatbot con RAG/LLM en una plataforma EdTech) y antes en fintech/insurtech. Estoy buscando mi próximo rol de PM remoto y quería preguntarte si hay vacantes abiertas en tu radar o el mejor camino para aplicar. ¿Tenés 15 minutos para charlar?

**4. Maria Jose Trejo Conde — Mercado Libre, Regional Talent Acquisition IT Senior Analyst** [tú — país no confirmado en tracker]
> Hola María José, te contacto porque lideras Talent Acquisition IT regional en Mercado Libre. Tengo 15+ años en Product Management (fintech, insurtech, EdTech con IA) y estoy evaluando mi próximo rol de PM remoto en LatAm. ¿Tendrías 15 minutos para comentarme si hay vacantes de producto abiertas o el mejor canal para aplicar?

**5. Bernardo Manzella — Globant, Head of People & Capacity Strategy (AI Studios)** [vos — Argentina]
> Hola Bernardo! Vi que liderás People & Capacity Strategy para AI Studios en Globant — doble match con mi perfil: PM con foco reciente en productos de IA (lideré un chatbot con RAG/LLM en una plataforma EdTech) y 15+ años en product management. Estoy evaluando mi próximo rol y me encantaría saber si hay vacantes en AI Studios o el mejor canal interno. ¿Tenés 15 minutos?

**6. Pedro Alejandro Santamarina — Mercado Libre, Sr. Product Development Manager** [vos — Argentina]
> Hola Pedro! Sos el contacto de Product más senior que tengo en Mercado Libre, así que te escribo directo. Vengo de 15+ años liderando producto (fintech, insurtech, EdTech con IA), el último rol liderando un chatbot con IA (RAG/LLM) a escala enterprise. Estoy evaluando mi próximo paso como PM y me encantaría 15 minutos para escuchar cómo ves el equipo de producto en MELI hoy, y si hay una vacante donde pueda calzar.

**Después de enviar estos 6 mensajes:** actualizá `rastreador-conexiones.md` con la fecha de envío de cada uno. Sin esa actualización, el sistema no puede detectar respuestas ni generar recordatorios a los 5+ días — es exactamente el gap que viene bloqueando esta sección desde el 25/09.

---

## Reconexión — Conexiones Existentes en Empresas con Gap (<4 conexiones)

Conexiones reales ya establecidas, no nuevas solicitudes — el próximo paso es reconectar, no pedir.

- **Elena Yndurain** (Microsoft, Director AI Product Management) — cubierta arriba como pedido de referido directo por relevancia altísima.
- **Melina Ruggeri** (Salesforce, LATAM Recruiting Senior Manager) — cubierta arriba.
- **Pablo Perez** (Apple, AIML) — marcado "Prioridad — rol de IA/ML" en el tracker, sin acción tomada aún. Candidato para el próximo lote si no hay respuesta de los 6 de arriba.
- **Alejandro Medici** (Amazon/AWS, Startup Solution Architect) — conexión antigua (2013), evaluar reconectar con mensaje de reactivación de red antes de pedir nada.

---

## Resumen del Día

- 0 solicitudes de conexión nuevas generadas (limitación estructural sin resolver — sin acceso a búsqueda de LinkedIn, 5ta sesión seguida señalándolo). Acción pendiente del usuario: pegar resultados de LinkedIn con el prompt de arriba.
- 0 seguimientos de conexiones aceptadas (sin solicitudes en curso registradas en el tracker).
- 6 pedidos de referido iniciales redactados y listos para enviar — usan datos 100% reales del tracker y de `biblioteca-experiencias.md`. Sin cambios de contenido respecto al 25/09 porque no hay evidencia de que se hayan enviado (el tracker sigue sin fecha de envío para ninguno).
- 0 recordatorios de referido (sin pedidos previos registrados con fecha).
- **Bottleneck persistente:** `rastreador-conexiones.md` lleva 46 días sin actualizarse. El sistema tiene research y mensajes listos (2 CVs adaptados para Stripe/VTEX del 03/09, 6 pedidos de referido redactados desde el 25/09) pero cero evidencia de ejecución. El cuello de botella no es de generación de contenido — es de envío y registro por parte del usuario.
