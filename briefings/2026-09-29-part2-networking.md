# Parte 2: Networking - Martes, 29 de septiembre de 2026

## Nota Metodológica (leer antes de usar el output de hoy)

El tracker de conexiones (`rastreador-conexiones.md`) solo contiene conexiones de **primer grado ya existentes** (importadas del CSV de LinkedIn), no tiene acceso a búsqueda de personas de 2do/3er grado. Este entorno tampoco tiene acceso directo a LinkedIn (ni browser, ni API). Para no violar la regla anti-fabricación de `CLAUDE.md` ("NUNCA fabricar experiencia... habilidades, proyectos ni métricas" — el mismo principio se extiende acá a no inventar personas reales para pedidos de conexión), las 19 solicitudes de abajo se armaron con **nombres, roles y empresas reales, verificados vía `WebSearch` contra perfiles públicos de LinkedIn indexados** (título + empresa visibles en el snippet de búsqueda). No son 2do grado confirmado en tu red — son personas reales identificadas por research, no contactos existentes.

**Limitaciones honestas de este método:**
- No hay forma de confirmar en qué grado de conexión están respecto a tu red real, ni si el "punto de conexión" (rol específico, foco del producto) sigue vigente hoy.
- Para varias empresas remote-friendly prioritarias (Stripe LATAM/GPTN específicamente, Atlassian con foco LatAm) no se encontraron perfiles con suficiente especificidad verificada — no se fuerza el match. Ver "Gaps sin cubrir" al final.
- Se entregan **19 de las 25 solicitudes por defecto**, no 25 — por la misma disciplina de precisión sobre volumen que ya aplicó el briefing de Roles hoy: mejor menos con research real que completar el número con nombres débiles o no verificados.
- Tratamiento vos/tú/inglés: se usó inglés para contactos fuera de países hispanohablantes de LatAm (Brasil, USA, Canadá, Europa) y **vos** para el único contacto confirmado en Argentina (Nicolás Ramos, Kavak) — la convención vos/tú de `CLAUDE.md` está pensada para países hispanohablantes; para Brasil se priorizó inglés por ser el estándar de outreach profesional cross-border en LinkedIn.

**Modo activo:** MODO REMOTO (confirmado por `plan-carrera.md`: "Remoto excluyente... filtro duro"). 15 de las 19 solicitudes (79%) van a empresas remote-friendly confirmadas en `empresas-objetivo.md` (Nubank, VTEX, Kavak, Deel, Shopify, GitLab, Linear, Twilio) — supera el mínimo de 50% requerido. No se activó MODO DIRECTOR+/EMPLEADO (el usuario no está actualmente empleado — gap de ~1 mes post-Amplifire, ver `plan-carrera.md`) ni MODO RETURNER (el gap real es de ~1 mes, encuadrado en `plan-carrera.md` como transición normal, no como gap de carrera que requiera reactivación de red).

---

## Solicitudes de Conexión (19 en total)

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Leandro Silvino | Nubank [remote-friendly] | Sr. Product Manager (ex-iFood, BV, Itaú) | Hi Leandro — your path through iFood, BV, Itaú and now Nubank's product org (plus mentoring at PROA) caught my eye. I'm a PM with 15+ yrs across fintech/healthtech, now specializing in AI (MSc, U. of Auckland). Would love to connect and learn about product at Nubank. |
| 2 | Maria Pamplona | Nubank [remote-friendly] | Sr. Product Manager & Squad Lead | Hi Maria — leading a squad as Sr PM at Nubank, one of LatAm's most product-driven fintechs, is impressive. I'm a PM with 15+ yrs in fintech/healthtech, now focused on AI (MSc, U. of Auckland). Would love to connect and hear about your experience there. |
| 3 | Felipe Laloni | Nubank [remote-friendly] | Senior Product Lead - Travel | Hi Felipe — Nubank's move into Travel as a product line is a great signal of where the org is headed, and leading that as Product Lead is a strong spot. I'm a PM with 15+ yrs across fintech/EdTech, now specializing in AI. Would love to connect. |
| 4 | Guilherme Augusto | Nubank [remote-friendly] | PM Manager / Staff PM (Under 18 products) | Hi Guilherme — Nubank's product for under-18s is a genuinely interesting segment to build for. I'm a PM with 15+ yrs in fintech/healthtech, now specializing in AI (MSc, U. of Auckland). Would love to connect and learn from your experience there. |
| 5 | Marília Hoffmann | VTEX [remote-friendly] | Product Manager (platform/integrations/APIs) | Hi Marília — your focus on platform, integrations, APIs and marketplace at VTEX lines up closely with product work I've done in fintech/telecom. I'm a PM with 15+ yrs leading global teams, now specializing in AI. Would love to connect. |
| 6 | Petrus Gomes | VTEX [remote-friendly] | Staff Product Manager | Hi Petrus — Staff PM at VTEX, a LatAm-born public company scaling enterprise ecommerce globally, is a strong trajectory. I'm a PM with 15+ yrs across fintech/healthtech/telecom, now specializing in AI (MSc, U. of Auckland). Would love to connect. |
| 7 | Matheus Furtado | VTEX [remote-friendly] | Senior Product Manager | Hi Matheus — Senior PM roles at VTEX carry real weight given its enterprise ecommerce scale. I'm a PM with 15+ yrs leading distributed product teams in fintech/healthtech, now specializing in AI. Would love to connect and hear about your work there. |
| 8 | Carolina Tourinho | VTEX [remote-friendly] | Product Manager | Hi Carolina — your work as PM at VTEX, one of the few LatAm-born public ecommerce platforms, stood out. I'm a PM with 15+ yrs across fintech/healthtech/telecom, now specializing in AI (MSc, U. of Auckland). Would love to connect. |
| 9 | Nicolás Ramos | Kavak [remote-friendly] | Sr. Product Manager, Fintech (Kuna), Buenos Aires | Hola Nicolás — vi que sos Sr PM en el área fintech (Kuna) de Kavak, desde Buenos Aires. Soy PM con 15+ años liderando producto en fintech/healthtech/telecom para equipos globales, ahora especializándome en IA (Master's, U. of Auckland). Me encantaría conectar. |
| 10 | Lucas Faraht | Deel [remote-friendly] | Lead Product Manager | Hi Lucas — leading product at Deel, the infrastructure behind global remote hiring, is a role I find genuinely relevant given my own history working remotely across LatAm/US/NZ. I'm a PM with 15+ yrs in fintech/healthtech, now specializing in AI. Would love to connect. |
| 11 | Ethan Welty | Deel [remote-friendly] | Senior Product Manager | Hi Ethan — Senior PM at Deel stood out given how closely it mirrors the remote/distributed model I've built my career around (LatAm, US, NZ, South Africa, India). I'm a PM with 15+ yrs in fintech/healthtech, now specializing in AI. Would love to connect. |
| 12 | Jonathan Zhao | Shopify [remote-friendly] | Senior Product Lead | Hi Jonathan — your work building Shopify's App Store ad platform as Senior Product Lead caught my attention. I'm a PM with 15+ yrs leading product for global distributed teams in fintech/healthtech, now specializing in AI. Would love to connect. |
| 13 | Mariana da Costa Melo | GitLab [remote-friendly] | (rol no confirmado en el snippet — ver nota) | Hi Mariana — GitLab's 100%-remote model since founding is the clearest example of what 'remote-first' really means, and I'd love to hear about product there from the inside. I'm a PM with 15+ yrs leading distributed teams, now specializing in AI. Would love to connect. |
| 14 | Alexandra Lapinsky Wilson | Linear [remote-friendly] | Product Manager | Hi Alexandra — Linear's reputation for product craft is well known in PM circles, and I'd love to hear what that looks like from the inside as PM there. I'm a PM with 15+ yrs across fintech/healthtech, now specializing in AI (MSc, U. of Auckland). Would love to connect. |
| 15 | Filip Budnik | Twilio [remote-friendly] | Product Manager | Hi Filip — building product at Twilio with a remote-first team resonates with how I've built my own career (LatAm, US, NZ, South Africa, India). I'm a PM with 15+ yrs in fintech/healthtech/telecom, now specializing in AI. Would love to connect. |
| 16 | Sophie Merrow | HubSpot | Senior Product Manager | Hi Sophie — Senior PM at HubSpot, a company known for genuinely product-led growth, is a strong spot to build from. I'm a PM with 15+ yrs across fintech/healthtech/telecom, now specializing in AI (MSc, U. of Auckland). Would love to connect. |
| 17 | Lukas Pleva | HubSpot | Group Product Manager | Hi Lukas — Group PM at HubSpot is a role I imagine sits right at the intersection of strategy and execution at scale. I'm a PM with 15+ yrs leading product for distributed global teams, now specializing in AI. Would love to connect and hear your take. |
| 18 | Ali BenCafu | Atlassian | Sr. Product Manager, AI adoption | Hi Ali — your focus on AI adoption as Sr PM at Atlassian lines up closely with where I'm headed: 15+ yrs in product (fintech/healthtech/telecom), now specializing in AI with an MSc from U. of Auckland. Would love to connect and compare notes. |
| 19 | John Murnen | Atlassian | Product Manager, Confluence AI | Hi John — working on Confluence AI as PM at Atlassian is squarely in the space I'm moving into. I'm a PM with 15+ yrs in fintech/healthtech/telecom, now specializing in AI (MSc, U. of Auckland). Would love to connect and hear about your work there. |

Todos los mensajes verificados por debajo de 300 caracteres (rango real: 229-270).

### Networking Virtual de Esta Semana (MODO REMOTO)

Unite a **Lenny's Newsletter community** (Lenny Rachitsky — la comunidad de PMs más activa a nivel global, fuerte presencia remota/distribuida) y comentá en 2-3 threads relevantes sobre transición a IA en producto o contratación remota LatAm. Como alternativa/complemento: **Product School Slack**, con canales específicos de LatAm.

---

## Seguimientos (Recién Conectados)

**Ninguno.** Se revisó `rastreador-conexiones.md` completo: la conexión más reciente registrada es del 17 de febrero de 2026 (Amazon/AWS) — no hay ninguna marcada como aceptada en las últimas 48 horas (última actualización general del archivo: 2026-08-13, 47 días sin refrescar). Si aceptaste alguna solicitud de las 19 de arriba (o de días previos) y no está reflejada acá, es porque el tracker no se actualizó — correr `/rastrear-postulaciones` o actualizar el archivo manualmente para que el próximo briefing la capture.

---

## Pedidos de Referido y Recordatorios

**Ninguno para hoy.** No existe `referral-tracker-template.md` en el repo, y no hay postulaciones registradas en `rastrear-postulaciones.md` (el archivo de datos no existe — confirmado también por el briefing de Parte 1 de hoy: "0 postulaciones enviadas registradas formalmente"). Sin pedidos de referido enviados ni postulaciones recientes, no hay nada que recordar o empujar hoy.

**Lo que sí vale la pena activar en cambio** (ya señalado por `rastreador-conexiones.md` en su sección de "Gap de Cobertura", con datos 100% reales de tu red de primer grado): tenés 6 conexiones de alta prioridad ya existentes sin activar hace 47+ días. Los dos más accionables hoy:
- **Elena Yndurain** (Microsoft) — Director AI Product Management, el match más directo con tu especialización en IA.
- **Virginia Silvero** (Globant) — Regional Recruiter Lead, South of LatAm.

Correr `/pedir-referido` para cualquiera de estos dos tendría mayor conversión esperada que las 19 solicitudes nuevas de arriba, porque ya son contactos de primer grado confirmados en tu red real — no research externo.

---

## Gaps Sin Cubrir (para transparencia, no para completar hoy)

- **Stripe (LATAM/GPTN team)** — el candidato de mejor fit de modalidad de todo el sistema según el briefing de Roles de hoy, pero no se encontró ningún perfil público verificable de un PM actual en ese equipo específico vía `WebSearch`. Requiere apertura manual de LinkedIn por el usuario.
- **Anthropic, HubSpot (con foco LatAm específico), Mercado Libre (nuevos hallazgos más allá de los 16 ya conectados)** — sin perfiles nuevos suficientemente específicos encontrados hoy.
- Big Tech con sponsorship (Amazon, Meta, Microsoft, Google, Apple) — deprioritizado para esta ronda de networking porque `empresas-objetivo.md` los marca como "roles mayormente presenciales/híbridos en HQ", lo que choca con el filtro duro de modalidad remota de `plan-carrera.md`.

---

## Próxima Actualización de `rastreador-conexiones.md`

Si envías estas 19 solicitudes manualmente en LinkedIn, actualizá el tracker (nombre, empresa, fecha, estado "solicitada") para que el briefing de mañana pueda detectar aceptaciones en la ventana de 48h y generar los seguimientos correspondientes.
