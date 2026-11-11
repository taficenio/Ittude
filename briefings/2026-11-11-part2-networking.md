# Parte 2: Networking - Miércoles, 11 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado, 2.092 conexiones totales importadas). **Última actualización real: 2026-08-13 — 90 días sin tocar** (confirmado vía `git log` sobre el archivo; el único commit que lo tocó desde entonces fue la carga inicial del repo el 2026-10-26, sin cambio de contenido).
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera — no aplica modo career-changer.
- **Modo Director+ / Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes; búsqueda activa; 0 postulaciones en 94 días per `briefings/2026-11-11-part1-roles.md`).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre roles), no un gap de carrera extendido que requiera reactivación de red.

---

## Solicitudes de Conexión (0 de 25 listas para enviar)

### Qué se intentó hoy

Se corrieron 3 búsquedas vía `WebSearch`: (1) re-verificación de la pista pendiente más vieja, **Carlos Vilches (NotCo)**, y (2)-(3) dos empresas de Tier 1 todavía sin búsqueda de personas intentada en corridas anteriores, **Nubank** y **VTEX**.

- **Carlos Vilches (NotCo)** — mismo resultado inconcluso que en corridas previas (desde 2026-11-04, re-verificado también el 2026-11-10): el perfil `cl.linkedin.com/in/carlosvilman` sigue describiéndose como "Head of Product Management @ NotCo", pero aparecen dos URLs casi idénticas sin que se pueda confirmar cuál es la vigente, y una señal contradictoria (un artículo que nombra a Aadit Patel como SVP de Producto de NotCo) que no permite descartar que el título esté desactualizado. [⚠️ NO VERIFICADO — misma pista sin resolver, ahora 7 días.]
- **Nubank** — la búsqueda devolvió dos perfiles de LinkedIn potencialmente relevantes (un rol de "Product Operations Senior Manager" en Argentina, y un "Product Manager" en Brasil), pero el resumen de la herramienta no expone nombre completo ni URL verificable para ninguno de los dos, y ninguno confirma explícitamente elegibilidad remota LatAm. Sin un nombre y perfil confirmables, no hay base para generar un mensaje — se descarta como hallazgo, no se fuerza una identidad.
- **VTEX** — único resultado con nombre (Julieta C., Buenos Aires) describe trabajo de canal/eCommerce con marcas y retailers que usan VTEX, no un cargo de Product Manager dentro de VTEX — mismo patrón de falso positivo ya documentado en `rastreador-conexiones.md` (ej. "Esther Sack - Agile Coach, partner de Salesforce, no empleada"). Se descarta.

Generar un mensaje de conexión citando un rol o dato no confirmado violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar cada pista con honestidad y dejarla pendiente de verificación humana — misma política aplicada en todas las corridas anteriores de Parte 2.

**Pistas pendientes acumuladas (sin verificar por el usuario):**
- Carlos Vilches (cl.linkedin.com/in/carlosvilman) — "Head of Product Management @ NotCo" (desde 2026-11-04, re-verificado sin éxito el 2026-11-10 y hoy — 7 días).
- Anamaría Barrera — "Twilio Talent Partner" vía stackforce.co, no LinkedIn directo (desde 2026-11-04 — 7 días).
- América Soto (Bitso, mx.linkedin.com/in/asotoh) — vigencia actual no confirmada (desde 2026-11-05 — 6 días).
- Pia Fajardo — "Group Product Manager - Payments" en Ualá (vía village.ai, no LinkedIn directo, desde 2026-11-06 — 5 días).
- Mayra Sciarrillo — "Chief Product Officer" en Ualá (vía theorg.com, no LinkedIn directo, desde 2026-11-06 — 5 días).
- María Sendra (ar.linkedin.com/in/mariasendra), Katheryn Rivera Lizano (ec.linkedin.com) — sin empresa objetivo confirmada (desde 2026-11-09 — 2 días).

**Empresas con búsqueda agotada hoy sin lead utilizable (sumadas a las 14 ya agotadas en corridas previas):** Nubank, VTEX.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Remote.com, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Bitso.

Sin cambios respecto a la asignación de corridas anteriores — sigue siendo el plan de referencia a la espera de que haya al menos una persona verificada por empresa.

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| — | *Sin personas verificadas hoy — tabla vacía por diseño, ver pistas pendientes arriba* | | | |

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable y, cuando lo hace, a menudo omite el nombre exacto o la URL verificable (como pasó hoy con Nubank). Ya se agotaron 16 empresas candidatas (14 de corridas previas + Nubank y VTEX hoy) sin producir un lote verificable completo. La vía más rápida para completar el lote de 25 sigue siendo:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Verificar manualmente las 6 pistas acumuladas (ver lista arriba).
3. Pegar nombre, rol y cualquier post reciente de esa persona, y ejecutar `/solicitud-conexion [lote]` — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, las dos comunidades definidas en CLAUDE.md para la función de PM:
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2.092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker sigue siendo del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **90 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en `plantillas/template-rastreador-referidos.md` (existe solo como plantilla vacía, sin instancias completadas). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones en 94 días del sistema, confirmado en `briefings/2026-11-11-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (3 búsquedas intentadas hoy: 1 re-verificación sin éxito, 2 empresas nuevas sin lead utilizable) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables con nombre+URL completos; 16 empresas candidatas ya agotadas |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 90 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 94 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, redactados el 2026-11-02, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** verificar manualmente las 6 pistas acumuladas (Carlos Vilches - NotCo, Anamaría Barrera - Twilio, América Soto - Bitso, Pia Fajardo - Ualá, Mayra Sciarrillo - Ualá, María Sendra y Katheryn Rivera Lizano) en LinkedIn y, si son reales y vigentes, decirle al sistema para generar sus mensajes; enviar los 6 pedidos de charla de 15 minutos ya redactados; y actualizar `rastreador-conexiones.md` (90 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos pendientes reales. Esta es otra corrida consecutiva de Parte 2 sin ningún envío humano registrado — el cuello de botella sigue siendo la activación, no la generación de contenido. Con 16 empresas remote-friendly/Tier 1 ya agotadas sin resultado utilizable en `WebSearch` sin login, vale la pena priorizar en la próxima corrida la verificación manual de las 6 pistas acumuladas por sobre seguir sumando empresas nuevas a la búsqueda.
