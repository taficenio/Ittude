# Parte 2: Networking - Jueves, 5 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado, 2.092 conexiones totales importadas). **Última actualización: 2026-08-13 — 84 días sin tocar.**
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera (no aplica modo career-changer).
- **Modo Director+/Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes, búsqueda activa, 0 postulaciones en 88 días per `briefings/2026-11-05-part1-roles.md`).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro. El lote de abajo asigna ≥50% a empresas remote-friendly confirmadas y suma sugerencia de comunidad virtual.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre roles), no un gap de carrera extendido.

---

## Solicitudes de Conexión (0 de 25 listas para enviar — ver intento de esta corrida)

### Qué se intentó hoy

Se corrieron 8 búsquedas vía WebSearch hoy, cubriendo empresas con gap de cobertura no probadas en corridas anteriores (2026-10-13, -14, 2026-11-02 a -04): **Remote.com, Zoom, Vercel, Linear** (remote-friendly confirmadas, prioridad Modo Remoto) y **Salesforce** (ya tiene 2 conexiones, igual cuenta como gap <4) del lado remote-friendly; **Rappi, iFood, Bitso** del lado Tier 2 LatAm. Mismo resultado estructural que las corridas previas: el motor de búsqueda no respeta de forma confiable `site:linkedin.com/in`, y la mayoría de resultados son bolsas de empleo (BuiltIn, Jobgether, Greenhouse, CryptoJobsList), páginas de agregadores (theorg, village.ai, remotar.com.br) o perfiles donde el título, la empresa y la vigencia actual no quedan claramente vinculados en el snippet.

**Señales parciales, NO verificadas — requieren confirmación manual antes de generar cualquier mensaje:**
- **América Soto** (mx.linkedin.com/in/asotoh) — el snippet la describe como Product Manager y lista Bitso en su experiencia, pero no confirma que Bitso sea su empleador *actual* ni la vigencia del cargo. [⚠️ NO VERIFICADO.]
- **Nico Botti** (ar.linkedin.com/in/nicobotti) — descrito como "Salesforce Delivery Manager" en Argentina con 6+ años liderando implementaciones, que dice estar abierto a roles de Product Manager. No es un PM actual de Salesforce — es un partner/implementador que usa la herramienta Salesforce, el mismo tipo de falso positivo que el tracker ya descartó para "Wise"/"Meta"/"Block". [⚠️ NO VERIFICADO — descartado como match real, no cuenta para el lote.]
- Remote.com, Zoom, Vercel, Linear, Rappi, iFood: ningún resultado produjo un par nombre+rol+empresa objetivo suficientemente claro y vigente. El resultado más cercano por empresa:
  - Zoom: todos los roles LatAm visibles son Sales/CS, no producto; ningún perfil de LinkedIn con esa combinación.
  - Vercel: un perfil de Bogotá apareció pero es irrelevante (recruiter de Salesforce, no Vercel).
  - Linear: los roles propios de Linear son Europa/Norteamérica, sin indicio de elegibilidad LatAm; cero perfiles.
  - Rappi: único perfil argentino con Rappi en su historial (Facundo Ozan) es Product *Designer*, no Product Manager.
  - iFood: dos perfiles brasileños aparecieron (Ottis - Alberto Brant, Bruna Griebeler) pero son Brasil, no LatAm remoto elegible para Argentina, y el foco de hoy fue completar gaps con mix de seniority, no agregar otro país sin verificar fit geográfico primero.

Generar un mensaje de conexión citando un rol o dato no confirmado violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar la pista con honestidad y dejarla pendiente de verificación humana — misma política aplicada en las 4 corridas anteriores de Parte 2.

**Pistas pendientes acumuladas (de corridas previas, aún sin verificar por el usuario):**
- Carlos Vilches (cl.linkedin.com/in/carlosvilman) — "Head of Product Management @ NotCo" (desde 2026-11-04).
- Anamaría Barrera — "Twilio Talent Partner" vía stackforce.co, no LinkedIn directo (desde 2026-11-04).
- América Soto (Bitso) — nueva de hoy.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

Para cumplir el requisito de Modo Remoto (≥50% del lote a empresas remote-friendly confirmadas), la asignación de 1 persona por empresa sería:

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Remote.com, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Bitso.

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable, y ya lleva 5 corridas consecutivas (2026-10-13, -14, 2026-11-02, -03, -04, -05) sin producir un lote verificable por esta vía. La vía más rápida para completar el lote de 25 sigue siendo:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Verificar manualmente a Carlos Vilches (NotCo), Anamaría Barrera (Twilio) y América Soto (Bitso) en LinkedIn directamente.
3. Pegar nombre, rol y cualquier post reciente de esa persona, y ejecutar `/solicitud-conexion [lote]` — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, las dos comunidades definidas en CLAUDE.md para la función de PM:
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2.092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker sigue siendo del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **84 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en `plantillas/template-rastreador-referidos.md` (existe solo como plantilla vacía, sin instancias completadas). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones en 88 días del sistema, confirmado en `briefings/2026-11-05-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (8 búsquedas intentadas hoy, 1 pista nueva sin verificar + 1 descartada por falso positivo) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 84 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 88 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, redactados el 2026-11-02, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** verificar manualmente a Carlos Vilches (NotCo), Anamaría Barrera (Twilio) y América Soto (Bitso) en LinkedIn y, si son reales y vigentes, decirle al sistema para generar sus mensajes; enviar los 6 pedidos de charla de 15 minutos ya redactados; y actualizar `rastreador-conexiones.md` (84 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos pendientes reales. Esta es la octava corrida consecutiva de Parte 2 sin ningún envío humano registrado — el cuello de botella sigue siendo la activación, no la generación de contenido.
