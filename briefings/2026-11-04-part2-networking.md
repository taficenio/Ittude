# Parte 2: Networking - Miércoles, 4 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado, 2.092 conexiones totales importadas). **Última actualización: 2026-08-13 — 83 días sin tocar.**
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera (no aplica modo career-changer).
- **Modo Director+/Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes, búsqueda activa, 0 postulaciones en 87 días per `briefings/2026-11-04-part1-roles.md`).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro. El lote de abajo asigna ≥50% a empresas remote-friendly confirmadas y suma sugerencia de comunidad virtual.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre roles), no un gap de carrera extendido.

---

## Solicitudes de Conexión (0 de 25 listas para enviar — ver intento de esta corrida)

### Qué se intentó hoy

Se corrieron 6 búsquedas vía WebSearch hoy, cubriendo empresas con gap de cobertura no probadas ayer (2026-11-03): Shopify, Twilio, Scale AI, NotCo, Zendesk, Betterfly. Mismo resultado estructural que ayer: el motor de búsqueda no respeta de forma confiable `site:linkedin.com/in`, así que la mayoría de resultados son bolsas de trabajo (Builtin, Jobera, Jobgether), directorios de terceros, o perfiles donde el título y la empresa objetivo no quedan claramente vinculados en el snippet.

**Señales parciales, NO verificadas — requieren confirmación manual antes de generar cualquier mensaje:**
- **Carlos Vilches** (cl.linkedin.com/in/carlosvilman) — aparece descrito como "Head of Product Management @ NotCo", Chile. Es el par nombre+rol más limpio de la corrida de hoy, pero el snippet no muestra fecha ni confirma vigencia actual. [⚠️ NO VERIFICADO.]
- **Anamaría Barrera** — aparece en un listado de talent marketplace (stackforce.co, no LinkedIn directo) como "Twilio Talent Partner" con un rol previo de Recruiter III en Colombia. [⚠️ NO VERIFICADO — fuente no es LinkedIn, doble motivo de cautela.]

Ningún otro resultado de hoy (Shopify, Scale AI, Zendesk, Betterfly) produjo un par nombre+rol+empresa objetivo suficientemente claro para pasar la regla de no fabricar contenido aplicada a personas reales. Generar un mensaje de conexión citando un rol o dato no confirmado violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar la pista con honestidad y dejarla pendiente de verificación humana.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

Para cumplir el requisito de Modo Remoto (≥50% del lote a empresas remote-friendly confirmadas), la asignación de 1 persona por empresa sería:

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Remote.com, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Stone Co.

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable. La vía más rápida para completar el lote de 25:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Verificar manualmente a Carlos Vilches (NotCo) y Anamaría Barrera (Twilio) en LinkedIn directamente.
3. Pegar nombre, rol y cualquier post reciente de esa persona, y ejecutar `/solicitud-conexion [lote]` — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, las dos comunidades definidas en CLAUDE.md para la función de PM:
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2.092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker sigue siendo del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **83 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en ningún tracker de referidos (`plantillas/template-rastreador-referidos.md` existe solo como plantilla vacía, sin instancias completadas). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones en 87 días del sistema, confirmado en `briefings/2026-11-04-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (6 búsquedas intentadas hoy, 2 pistas sin verificar) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 83 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 87 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, redactados el 2026-11-02, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** verificar manualmente a Carlos Vilches (NotCo) y Anamaría Barrera (Twilio) en LinkedIn y, si son reales y vigentes, decirle al sistema para generar sus mensajes; enviar los 6 pedidos de charla de 15 minutos ya redactados; y actualizar `rastreador-conexiones.md` (83 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos pendientes reales. Esta es la séptima corrida consecutiva de Parte 2 sin ningún envío humano registrado — el cuello de botella sigue siendo la activación, no la generación de contenido.
