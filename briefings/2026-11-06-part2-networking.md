# Parte 2: Networking - Viernes, 6 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado, 2.092 conexiones totales importadas). **Última actualización: 2026-08-13 — 85 días sin tocar.**
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera (no aplica modo career-changer).
- **Modo Director+/Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes, búsqueda activa, 0 postulaciones en 89 días per `briefings/2026-11-06-part1-roles.md`).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro. Ver más abajo por qué esto quedó sin poder cumplirse del todo hoy.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre roles), no un gap de carrera extendido.

---

## Solicitudes de Conexión (0 de 25 listas para enviar — sexta corrida consecutiva sin lote verificable)

### Qué se intentó hoy

Se corrieron 6 búsquedas vía WebSearch hoy, cubriendo empresas no probadas (o no agotadas) en corridas anteriores (2026-10-13, -14, 2026-11-02 a -05):

- **Automattic, Zapier, Buffer** — las tres empresas remote-first que CLAUDE.md nombra explícitamente como ejemplos de Modo Remoto además de las ya marcadas en `empresas-objetivo.md` (GitLab, Deel, Atlassian, Shopify, Remote.com — las 5 agotadas sin resultado en corridas previas, ver nota abajo).
- **Amazon** (reclutamiento LatAm) — empresa con conexiones existentes pero por debajo del umbral de 4 (3 conexiones).
- **Klarna** (Tier 2, Fintech Global, sin conexiones).
- **Ualá** (Tier 2, LatAm, sin conexiones).

Mismo resultado estructural que las 5 corridas previas: el motor de búsqueda no respeta de forma confiable `site:linkedin.com/in`, y la mayoría de resultados son postings de empleo (BuiltIn, WorkingNomads, Greenhouse, Jobgether), agregadores de terceros (theorg, village.ai, zoominfo, humantic.ai) o perfiles de LinkedIn donde el título, la empresa objetivo y la vigencia actual no quedan claramente vinculados en el snippet.

**Hallazgo relevante de hoy — las 5 empresas remote-friendly ya marcadas en `empresas-objetivo.md` (GitLab, Deel, Atlassian, Shopify, Remote.com) están agotadas:** fueron buscadas sin éxito en una o más corridas entre el 2026-10-13 y el 2026-11-05. Esto significa que, por quinto/sexto día consecutivo, **no hay forma de completar el requisito de Modo Remoto (≥50% del lote a empresas remote-friendly confirmadas) sin repetir búsquedas ya agotadas o sin ampliar el universo de empresas remote-friendly** — lo cual se intentó hoy con Automattic/Zapier/Buffer, nombradas explícitamente en CLAUDE.md, sin resultado verificable tampoco.

**Señales parciales, NO verificadas — requieren confirmación manual antes de generar cualquier mensaje:**
- **Pia Fajardo** — descrita (vía agregador village.ai, no LinkedIn directo) como "Group Product Manager - Payments" en Ualá, Argentina, desde jul 2025. [⚠️ NO VERIFICADO — fuente no es LinkedIn directo.]
- **Mayra Sciarrillo** — descrita (vía theorg.com, no LinkedIn directo) como Chief Product Officer en Ualá desde feb 2024. [⚠️ NO VERIFICADO — fuente no es LinkedIn directo, y un cargo C-level cambia el tipo de pedido posible (más indicado para networking ejecutivo que para solicitud de conexión estándar).]
- **Juan Pablo Cook** (ar.linkedin.com/in/juanpcook) — el snippet solo confirma que tiene conexiones en Automattic, no que trabaje ahí ni en qué rol. [⚠️ NO VERIFICADO.]
- Automattic, Zapier, Buffer, Amazon, Klarna: ningún resultado produjo un par nombre+rol+empresa objetivo suficientemente claro y vigente, directamente en LinkedIn.

Generar un mensaje de conexión citando un rol o dato no confirmado violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar la pista con honestidad y dejarla pendiente de verificación humana — misma política aplicada en las 5 corridas anteriores de Parte 2.

**Pistas pendientes acumuladas (de corridas previas, aún sin verificar por el usuario):**
- Carlos Vilches (cl.linkedin.com/in/carlosvilman) — "Head of Product Management @ NotCo" (desde 2026-11-04).
- Anamaría Barrera — "Twilio Talent Partner" vía stackforce.co, no LinkedIn directo (desde 2026-11-04).
- América Soto (Bitso, mx.linkedin.com/in/asotoh) — vigencia actual no confirmada (desde 2026-11-05).
- Pia Fajardo (Ualá) y Mayra Sciarrillo (Ualá) — nuevas de hoy.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

Dado que las 5 empresas remote-friendly marcadas en `empresas-objetivo.md` están agotadas en WebSearch, el plan de asignación se mantiene igual que en corridas anteriores a la espera de verificación manual (vía LinkedIn logueado):

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Remote.com, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Bitso.

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable, y ya lleva **6 corridas consecutivas** (2026-10-13, -14, 2026-11-02 a -06) sin producir un lote verificable por esta vía, habiendo agotado ya las 8 empresas remote-friendly candidatas (5 de `empresas-objetivo.md` + las 3 nombradas en CLAUDE.md). Repetir la misma búsqueda sobre las mismas empresas en corridas futuras tiene valor marginal decreciente. La vía más rápida para completar el lote de 25 sigue siendo:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Verificar manualmente a Pia Fajardo y Mayra Sciarrillo (Ualá), Carlos Vilches (NotCo), Anamaría Barrera (Twilio) y América Soto (Bitso) en LinkedIn directamente.
3. Pegar nombre, rol y cualquier post reciente de esa persona, y ejecutar `/solicitud-conexion [lote]` — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, las dos comunidades definidas en CLAUDE.md para la función de PM:
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2.092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker sigue siendo del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **85 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en `plantillas/template-rastreador-referidos.md` (existe solo como plantilla vacía, sin instancias completadas). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones en 89 días del sistema, confirmado en `briefings/2026-11-06-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (6 búsquedas intentadas hoy, 3 pistas nuevas sin verificar) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables; las 8 empresas remote-friendly candidatas ya están agotadas |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 85 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 89 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, redactados el 2026-11-02, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** verificar manualmente a Pia Fajardo y Mayra Sciarrillo (Ualá), Carlos Vilches (NotCo), Anamaría Barrera (Twilio) y América Soto (Bitso) en LinkedIn y, si son reales y vigentes, decirle al sistema para generar sus mensajes; enviar los 6 pedidos de charla de 15 minutos ya redactados; y actualizar `rastreador-conexiones.md` (85 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos pendientes reales. Esta es la **novena corrida consecutiva de Parte 2 sin ningún envío humano registrado** — el cuello de botella sigue siendo la activación, no la generación de contenido. Dado que la vía de WebSearch sin login ya se agotó sobre las 8 empresas remote-friendly candidatas, seguir corriendo esta Parte 2 sin que el usuario envíe al menos los 6 mensajes ya redactados o habilite acceso a LinkedIn no va a producir un resultado distinto al de hoy.
