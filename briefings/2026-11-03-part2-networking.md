# Parte 2: Networking - Martes, 3 de Noviembre de 2026

## Gate de Calidad

- `rastreador-conexiones.md`: datos reales (108 empresas cruzadas, 9 con conexiones de 1er grado). **Última actualización: 2026-08-13 — 82 días sin tocar.**
- `empresas-objetivo.md`: datos reales (108 empresas en 4 tiers, generado 2026-08-10).
- `plan-carrera.md`: datos reales.

Gate superado. Continúa el briefing completo.

## Detección de Modo

- **Función objetivo:** Product Manager / Product Owner (IC Senior, Lead/Head, o especialización en IA — tres caminos abiertos). Sin transición de carrera (no aplica modo career-changer).
- **Modo Director+/Empleado:** NO aplica — el usuario no está en nivel Director+ ni actualmente empleado (contrato en Amplifire terminó hace ~1 mes, búsqueda activa).
- **Modo Remoto:** SÍ aplica — `plan-carrera.md` marca "Remoto excluyente" como filtro duro. El lote de abajo asigna ≥50% a empresas remote-friendly confirmadas y suma sugerencia de comunidad virtual.
- **Modo Returner:** NO aplica — el gap de empleo real es de ~1 mes (transición normal), no un gap de carrera.

---

## Solicitudes de Conexión (0 de 25 listas para enviar — ver intento de esta corrida)

### Qué se intentó hoy (distinto de corridas anteriores)

A diferencia de corridas previas que señalaron el gap sin buscar, hoy se corrieron **23 búsquedas vía WebSearch** intentando encontrar perfiles reales de LinkedIn (reclutadores o PMs) en las empresas con gap de cobertura: Deel, GitLab, Atlassian, Shopify, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub, Remote.com, Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Stone Co.

**Resultado: ninguna búsqueda devolvió un perfil de LinkedIn verificable como empleado actual de la empresa objetivo en rol de Producto o Talent Acquisition.** El motor de búsqueda no respeta de forma confiable el operador `site:linkedin.com/in`, así que la mayoría de resultados fueron bolsas de trabajo (Greenhouse, Built-in, job boards) o perfiles de reclutadores LATAM genéricos sin afiliación confirmada a la empresa buscada.

**Única señal parcial, NO verificada — requiere confirmación manual antes de usar:**
- **Camilo Vargas** (co.linkedin.com/in/camilo-vargas-ahumada) — aparece descrito en los resultados como "Head of CX - Product Operations at Nubank", con actividad reciente sobre la expansión de Nubank en Argentina. [⚠️ NO VERIFICADO — el snippet de búsqueda puede estar desactualizado o mal inferido. Confirmar el perfil completo manualmente antes de generar cualquier mensaje.]
- **Juan Aragon** (ar.linkedin.com/in/juan-luis-aragon) — descrito como "Product Operations Senior Manager" con 10+ conexiones mutuas en Nubank. [⚠️ NO VERIFICADO — mismo motivo que arriba.]

Generar un mensaje de conexión de 300 caracteres citando un rol o dato personal no confirmado violaría la regla central del sistema aplicada a personas reales (CLAUDE.md: "NUNCA fabricar... NUNCA generar contenido genérico"). Se prefiere señalar la pista con honestidad y dejarla pendiente de verificación humana, no redactar el mensaje todavía.

### Asignación round-robin planificada (25 slots, lista para completar en cuanto haya personas verificadas)

Para cumplir el requisito de Modo Remoto (≥50% del lote a empresas remote-friendly confirmadas), la asignación de 1 persona por empresa sería:

**Remote-friendly confirmadas (14/25 = 56%):** Deel, GitLab, Atlassian, Salesforce, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub, Remote.com.
**Resto del lote, priorizando Tier 1 y luego Tier 2 LatAm (11/25):** Nubank, Anthropic, Stripe, HubSpot, Notion, Duolingo, Kavak, VTEX, Rappi, iFood, Stone Co.

### Cómo desbloquear esto en la próxima corrida

Esta sesión cloud no tiene navegador ni login de LinkedIn — solo búsqueda web pública, que indexa muy poco de LinkedIn de forma confiable. La vía más rápida para completar el lote de 25:

1. Correr una búsqueda de personas en LinkedIn (logueado) para 1-2 empresas del lote por día, con esta plantilla (la misma que usa `/solicitud-conexion`):
   > `"[Empresa]"` AND (`"Product Manager"` OR `"PM"` OR `"Talent Acquisition"` OR `"Recruiter"`) AND (`"LatAm"` OR `"Argentina"` OR `"Remote"`)
2. Pegar nombre, rol y cualquier post reciente de esa persona.
3. Ejecutar `/solicitud-conexion [lote]` con esos nombres — ahí el OS redacta los 25 mensajes personalizados con precisión.
4. Alternativa: habilitar Claude in Chrome o el navegador integrado para esta sesión, así una corrida futura puede buscar de punta a punta.

### Networking virtual de esta semana (Modo Remoto)

Dado el filtro remoto excluyente, sumar 2 canales virtuales esta semana en paralelo al outreach 1:1 (rotando respecto a Product School, Lenny y ADPList ya sugeridos en corridas de esta misma semana):
- **Unirte al Slack de Product School** y comentar en 2-3 threads recientes sobre AI Product Management o transiciones a roles remotos LatAm.
- **Unirte a la comunidad de Lenny** (Lenny's Newsletter/Slack) y comentar en 2-3 threads relevantes — alta concentración de hiring managers y PMs senior que contratan remoto.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguno.** `rastreador-conexiones.md` no registra ninguna transición "solicitada → conectada" con fecha — el archivo solo contiene fechas de conexión originales de la importación del CSV de LinkedIn (2,092 conexiones, cruzadas el 2026-08-13). La conexión más reciente de todo el tracker es del 19 de noviembre de 2025 (Sharik Garzón Terán, Mercado Libre) — muy fuera de cualquier ventana de 48hs contada desde hoy. El archivo lleva **82 días sin actualizarse**.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)

**Ninguno.** No hay registro de ningún pedido de referido enviado hasta la fecha en `rastreador-conexiones.md` ni en ningún tracker de referidos (no existe `referral-tracker-template.md` poblado en el repo). Sin fecha real de envío, no hay base para calcular un recordatorio de "5+ días sin respuesta".

### Nuevos Pedidos de Referido

Ningún rol fue postulado en las últimas 48 horas (0 postulaciones totales en 86 días del sistema, confirmado en `briefings/2026-11-03-part1-roles.md`), así que el disparador formal de esta sección no aplica.

**Acción de mayor apalancamiento disponible hoy (sin cambios respecto a corridas anteriores — sigue sin enviarse):** los 6 mensajes de pedido de charla de 15 minutos a las conexiones de 1er grado de mayor prioridad (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) ya están redactados completos en `briefings/2026-11-02-part2-networking.md`. No se reescriben acá para no generar versiones inconsistentes del mismo pedido — correr `/pedir-referido [nombre + rol]` si se necesita una versión nueva.

---

## Resumen de la corrida

| Sección | Generado | Motivo si no |
|---|---|---|
| Solicitudes de conexión nuevas | 0 de 25 (23 búsquedas intentadas, 2 pistas sin verificar) | Sin navegador/login de LinkedIn; búsqueda web pública no indexa perfiles confiables |
| Seguimientos a recién conectados | 0 | Tracker sin actualizar hace 82 días, sin datos de aceptaciones recientes |
| Recordatorios de referido (5+ días) | 0 | Nunca se envió un pedido de referido (0 postulaciones en 86 días) |
| Pedidos de referido nuevos | 0 (los 6 de siempre, ya redactados ayer, siguen sin enviarse) | Ver `briefings/2026-11-02-part2-networking.md` |

**Acción humana pendiente más urgente:** verificar manualmente a Camilo Vargas y Juan Aragon (Nubank) en LinkedIn y, si son reales y vigentes, decirle al sistema para generar sus mensajes; enviar los 6 pedidos de charla de 15 minutos ya redactados; y actualizar `rastreador-conexiones.md` (82 días sin tocar) para que las próximas corridas puedan detectar aceptaciones y pedidos pendientes reales.
