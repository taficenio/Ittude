# Parte 2: Networking - Jueves, 12 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado, 2.092 conexiones totales importadas). **Última actualización real de contenido: 2026-08-13 — 91 días sin tocar** (confirmado vía `git log`: el único commit que tocó el archivo desde entonces fue la carga inicial del repo el 2026-10-27, sin cambio de contenido).
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera — no aplica modo career-changer.
- **Modo Director+ / Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes; búsqueda activa; 0 postulaciones en 95 días per `briefings/2026-11-12-part1-roles.md`).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal entre roles), no un gap de carrera extendido.

---

## Solicitudes de Conexión (0 de 25 listas para enviar)

### Qué se intentó hoy

Se corrieron 2 búsquedas vía `WebSearch`, cubriendo dos empresas de Tier 1 todavía sin búsqueda de personas intentada en corridas anteriores: **Anthropic** y **Stripe**.

- **Anthropic** — el operador `site:linkedin.com/in` no filtró como se esperaba; los resultados son mayormente job boards de terceros (Singular, Arionkoder, Caylent) y dos perfiles de LinkedIn de Argentina (Ambar Franco, Sol Parnofiello) sin ningún rol o vínculo con Anthropic visible en el snippet. Caylent aparece como "charter member of Anthropic's Claude Partner Network" — es un partner, no Anthropic. Sin nombre y rol confirmables dentro de Anthropic, se descarta.
- **Stripe** — mismo patrón: resultados de job boards (incluyendo un rol de Technical Recruiter para expansión LatAm de Stripe, con ~930 días de antigüedad, probablemente cerrado) y perfiles sin confirmar. El único perfil de reclutamiento de Stripe encontrado está en Bucharest (EMEA), no LatAm. Un perfil de Argentina (Pedro Bontempi) aparece sin mención de Stripe en el snippet. Se descarta.

Generar un mensaje de conexión citando un rol o dato no confirmado violaría la regla central del sistema (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar cada pista con honestidad y dejarla pendiente de verificación humana — misma política aplicada en todas las corridas anteriores de Parte 2.

No se reintentó la re-verificación de las pistas pendientes acumuladas hoy: Carlos Vilches (NotCo) ya fue re-verificado sin éxito el 2026-11-04, 2026-11-10 y 2026-11-11 (tres intentos, mismo resultado inconcluso) — repetir una cuarta vez con la misma búsqueda pública sin login no cambiaría el resultado. Se priorizó usar las 2 búsquedas de hoy en empresas nuevas en su lugar.

**Pistas pendientes acumuladas (sin verificar por el usuario):**
- Carlos Vilches (cl.linkedin.com/in/carlosvilman) — "Head of Product Management @ NotCo" (desde 2026-11-04, re-verificado sin éxito 3 veces — ahora 8 días sin resolver).
- Anamaría Barrera — "Twilio Talent Partner" vía stackforce.co, no LinkedIn directo (desde 2026-11-04 — 8 días).
- América Soto (Bitso, mx.linkedin.com/in/asotoh) — vigencia actual no confirmada (desde 2026-11-05 — 7 días).
- Pia Fajardo — "Group Product Manager - Payments" en Ualá (vía village.ai, no LinkedIn directo, desde 2026-11-06 — 6 días).
- Mayra Sciarrillo — "Chief Product Officer" en Ualá (vía theorg.com, no LinkedIn directo, desde 2026-11-06 — 6 días).
- María Sendra (ar.linkedin.com/in/mariasendra), Katheryn Rivera Lizano (ec.linkedin.com) — sin empresa objetivo confirmada (desde 2026-11-09 — 3 días).

**Empresas con búsqueda agotada hoy sin lead utilizable (sumadas a las 16 ya agotadas en corridas previas):** Anthropic, Stripe. Total acumulado: **18 empresas agotadas sin resultado utilizable** vía búsqueda web pública sin login de LinkedIn.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Remote.com, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Bitso.

Sin cambios respecto a la asignación de corridas anteriores — sigue siendo el plan de referencia a la espera de que haya al menos una persona verificada por empresa.

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| — | *Sin personas verificadas hoy — tabla vacía por diseño, ver pistas pendientes arriba* | | | |

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable y, cuando lo hace, a menudo omite el nombre exacto, el rol vigente o la URL verificable (como pasó hoy con Anthropic y Stripe). Ya se agotaron 18 empresas candidatas sin producir un lote verificable completo, en 13 corridas consecutivas de Parte 2. La vía más rápida para completar el lote de 25 sigue siendo:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Verificar manualmente las 6 pistas acumuladas (ver lista arriba), la más vieja con 8 días sin resolver.
3. Pegar nombre, rol y cualquier post reciente de esa persona, y ejecutar `/solicitud-conexion [lote]` — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, las dos comunidades definidas en CLAUDE.md para la función de PM:
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2.092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker sigue siendo del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **91 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en `plantillas/template-rastreador-referidos.md` (existe solo como plantilla vacía, sin instancias completadas). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones en 95 días del sistema, confirmado en `briefings/2026-11-12-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (2 búsquedas intentadas hoy, ambas sin lead utilizable) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables con nombre+rol+URL completos; 18 empresas candidatas ya agotadas |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 91 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 95 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, redactados el 2026-11-02, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** esta es la **decimotercera corrida consecutiva de Parte 2 sin ningún envío humano registrado**. El cuello de botella ya no es de generación de contenido — es de activación: (1) enviar los 6 mensajes de charla de 15 minutos ya redactados desde hace 10 días (`briefings/2026-11-02-part2-networking.md`), (2) verificar manualmente las 6 pistas acumuladas (la más vieja, Carlos Vilches en NotCo, con 8 días sin resolver), y (3) actualizar `rastreador-conexiones.md` (91 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos reales. Con 18 empresas remote-friendly/Tier 1 ya agotadas sin resultado utilizable en `WebSearch` sin login, seguir sumando empresas nuevas día tras día sin que el usuario actúe sobre lo ya redactado no va a cambiar el resultado de esta sección — vale la pena pausar la expansión de búsqueda hasta que haya señal de actividad humana sobre lo pendiente.
