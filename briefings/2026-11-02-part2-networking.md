# Parte 2: Networking - Lunes, 2 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado). **Última actualización: 2026-08-13 — 81 días sin tocar.**
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera (no aplica modo career-changer).
- **Modo Director+/Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes, búsqueda activa).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro. Se prioriza el lote hacia empresas remote-friendly confirmadas y se agrega sugerencia de comunidad virtual.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre contratos), no un gap de carrera que amerite reactivación de red tipo "returner". Se trata como networking activo estándar.

---

## Solicitudes de Conexión (0 generadas — ver limitación de herramienta)

**No se generaron las 25 solicitudes de conexión nuevas en esta corrida.** Razón: identificar personas reales y específicas en las empresas con gap de cobertura (las 99 de 108 empresas objetivo sin ninguna conexión de 1er grado, según `rastreador-conexiones.md`) requiere buscar/navegar LinkedIn para encontrar prospects verificables con nombre, rol y punto de conexión reales. Esta sesión cloud automatizada no tiene acceso a navegador ni a LinkedIn. Inventar 25 nombres, roles o "puntos de conexión" sin esa verificación violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar experiencia... NUNCA generar contenido genérico") — en este caso aplicada a personas reales, no solo a la experiencia del usuario. Se prefiere señalar el gap con honestidad, siguiendo el mismo criterio que usó la Parte 1 de hoy al marcar roles como "no se pudo verificar" en lugar de inventar vacantes.

### Empresas con gap de cobertura confirmado (fuente: `rastreador-conexiones.md`)

**Cero conexiones (Tier 1, prioridad alta):** Nubank, Anthropic, Deel, Stripe, GitLab, HubSpot, Notion, Duolingo, Kavak, VTEX.
**Cobertura parcial (<4 conexiones):** Amazon/AWS (3), Apple (2), Google (2), Salesforce (2), Atlassian (1).
**Además:** 89 empresas adicionales de Tier 2-4 sin ninguna conexión de 1er grado (ver `empresas-objetivo.md` para el listado completo).

### Recomendación para la próxima corrida

Buscar manualmente en LinkedIn 5-10 prospects reales por empresa prioritaria (filtro: empresa + "Product" + LatAm/remoto) y correr `/solicitud-conexion [lote]` con esos nombres reales — ahí el OS sí puede redactar los 25 mensajes personalizados de menos de 300 caracteres con precisión. Alternativa: conectar esta sesión a un navegador (Claude in Chrome o browser integrado) para que la búsqueda se pueda hacer de punta a punta en una corrida futura.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, sumar 2 canales virtuales esta semana en paralelo al outreach 1:1:
- **Unirte al Slack de Product School** y comentar en 2-3 threads relevantes sobre AI Product Management o transiciones a roles LatAm-remoto.
- **Unirte a la comunidad de Lenny (Lenny's Newsletter/Slack)** y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Recién Conectados)

**Ninguno.** `rastreador-conexiones.md` no registra ningún cambio de estado "solicitada → conectada" porque no tiene datos de los últimos 2 días — la última actualización real del archivo es del 2026-08-13 (81 días). No hay manera de verificar aceptaciones recientes con el archivo en este estado.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** Según `historial-entrevistas.md` y `rastreador-conexiones.md`, no hay registro de ningún pedido de referido enviado hasta la fecha (0 postulaciones enviadas en 85 días, por `briefings/2026-11-02-part1-roles.md`). No hay nada que recordar todavía.

### Nuevos Pedidos de Referido — acción recomendada del día

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones totales), así que el disparador literal de esta sección no aplica tampoco. Pero `rastreador-conexiones.md` ya señala esto como **el cuello de botella de mayor apalancamiento del sistema** y deja priorizados 6 contactos reales de 1er grado en empresas Tier 1 sin gap de cobertura (Globant, Mercado Libre) — la acción de más alto ROI disponible hoy, con datos 100% verificados (nombre, rol y empresa reales de `rastreador-conexiones.md`). Se redactan los 6 mensajes de pedido de charla/referido para que el usuario los envíe hoy:

- **Elena Yndurain** (Director AI Product Management, Microsoft): "Hola Elena! Hace rato no hablamos — te sigo desde que estás liderando AI Product Management en Microsoft, justo el cruce que yo también vengo armando (vengo de liderar un chatbot con RAG/LLM en producción en Amplifire, más un Master en IA recién terminado). Estoy evaluando mi próximo paso en Product y Microsoft está en mi radar. ¿Tendrías 15 minutos para charlar y, si tiene sentido, contarme cómo ves el equipo hoy?"

- **Virginia Silvero** (Regional Recruiter Lead, South of LatAm, Globant): "Hola Virginia! Más de 15 años desde que nos conectamos — vi que seguís liderando reclutamiento regional en Globant para el sur de LatAm. Estoy en búsqueda activa de mi próximo rol de Product (Senior PM/PO, abierto también a Lead) y Globant es de mis empresas prioritarias. ¿Tenés 15 minutos para una charla rápida sobre cómo está el pipeline de Product hoy?"

- **Melina Ruggeri** (LATAM Recruiting Senior Manager, Salesforce): "Hola Melina! Hace tiempo que no hablamos — veo que seguís como Senior Manager de Recruiting LATAM en Salesforce. Estoy en búsqueda activa de mi próximo rol de Product Manager/Owner y Salesforce está entre mis empresas objetivo. ¿Tendrías 15 minutos para ponernos al día y contarme cómo está el área de Producto hoy?"

- **Maria Jose Trejo Conde** (Regional Talent Acquisition IT Senior Analyst, Mercado Libre): "Hola Maria Jose! Hace tiempo que no hablamos — te sigo en tu rol de Talent Acquisition IT regional en Mercado Libre. Estoy evaluando mi próximo paso en Product (Senior PM/PO) y MeLi es una de mis prioridades. ¿Tendrías 15 minutos para una charla rápida sobre cómo está el área de Producto hoy?"

- **Bernardo Manzella** (Head of People & Capacity Strategy, AI Studios, Globant): "Hola Bernardo! Hace mucho no hablamos — vi que estás liderando People & Capacity Strategy en Globant AI Studios, justo el cruce entre Producto e IA en el que vengo especializándome (Master en IA + experiencia reciente liderando un chatbot con RAG/LLM en Amplifire). Estoy evaluando mi próximo rol y Globant/AI Studios está en mi radar. ¿Tendrías 15 minutos para charlar?"

- **Pedro Alejandro Santamarina** (Sr. Product Development Manager, Mercado Libre): "Hola Pedro! Hace tiempo que no hablamos — seguís liderando Product Development en Mercado Libre. Estoy en búsqueda activa de mi próximo rol de Product (Senior PM/PO, con foco reciente en IA) y MeLi está entre mis prioridades. ¿Tendrías 15 minutos para una charla y, si tiene sentido en el camino, contarme cómo ves el área hoy?"

**Nota:** estos no son pedidos de referido directos (todavía no hay rol/postulación concreta a la cual atar un referido), son pedidos de charla de 15 minutos — el paso previo correcto según la filosofía del sistema ("Referidos antes que postulaciones frías"). Una vez agendada la charla, correr `/pedir-referido` con el rol específico si la conversación lo justifica.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 | Sin acceso a LinkedIn/navegador para verificar prospects reales |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 81 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 85 días) |
| Pedidos de referido nuevos | 6 | Generados desde datos 100% verificados en `rastreador-conexiones.md` |

**Acción humana pendiente más urgente:** actualizar `rastreador-conexiones.md` (81 días sin tocar) y, si es posible, habilitar acceso a navegador/LinkedIn para que la próxima corrida pueda generar las 25 solicitudes de conexión reales en vez de señalar el gap.
