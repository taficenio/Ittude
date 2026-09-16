# Parte 2: Networking - Miércoles, 16 de septiembre de 2026

## Gate de Calidad — Estado de Contexto

- `rastreador-conexiones.md`: datos reales (2,092 conexiones LinkedIn cruzadas contra 108 empresas objetivo). Última actualización: 2026-08-13 (34 días sin cambios — ninguna de las solicitudes de conexión generadas en briefings previos está marcada como enviada).
- `empresas-objetivo.md`: datos reales, 108 empresas rankeadas. Última actualización: 2026-08-10.
- `plan-carrera.md`: datos reales. Función objetivo: Product Manager/Owner (IC senior, Lead/Head, o especialización IA). **Modalidad: remoto excluyente** (filtro duro). Mercado: Argentina, LatAm, USA, Canadá.

Los tres archivos requeridos tienen contenido real — se continúa con el briefing completo.

**Modo activado: MODO REMOTO** (plan-carrera.md marca "remoto excluyente" como filtro duro). No se activa modo Director+/empleado (el usuario no está empleado actualmente — gap de ~1 mes desde que terminó Amplifire) ni modo Returner (el gap de ~1 mes se documenta en plan-carrera.md como transición normal, no como gap de carrera extendido).

**Aviso de bloqueo estructural (heredado de Parte 1):** `WebFetch` sigue bloqueado (`EGRESS_BLOCKED`) contra dominios de LinkedIn — verificado hoy contra `linkedin.com`. Esto significa que ningún contacto nuevo de esta lista pudo verificarse abriendo su perfil real; todo surge de snippets de `WebSearch` (nombre + rol + empresa, a veces país). Se optó por **no fabricar** puntos de conexión específicos (universidad compartida, conexión mutua) que no se pueden verificar — cada mensaje usa únicamente el rol/empresa real confirmado por búsqueda, que sí es un dato verificable.

---

## Solicitudes de Conexión (18 de 25 objetivo — ver nota de shortfall)

**Cobertura round-robin, priorizando remote-friendly:** las 18 personas identificadas trabajan en 10 empresas objetivo con gap de cobertura (0-3 conexiones en `rastreador-conexiones.md`), **todas ellas remote-friendly confirmadas** en `empresas-objetivo.md` (GitLab 100% remoto, Deel full-remote, Nubank/VTEX remoto regional LatAm, HubSpot/Twilio/Zendesk/GitHub/PayPal/Shopify/Anthropic con contratación remota LatAm o global confirmada) — 100% del lote cumple el mínimo de 50% remote-friendly exigido por MODO REMOTO.

**Idioma:** mensajes en inglés por default (la mayoría son reclutadores/as de equipos globales, y varias empresas LatAm del lote son de Brasil — portugués, no español, por lo que aplicar vos/tú hubiera sido un error). Excepción: Andrés Miguel Díaz (Zendesk, ubicación confirmada México vía URL de LinkedIn) recibe el mensaje en español con tratamiento de tú.

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Ben Cowdry | GitLab | Recruitment Manager | Hi Ben, saw you lead Recruitment at GitLab -- still the clearest proof that 100%-remote works at scale. I'm a Senior PM (AI/LLM products) based in Argentina with a fully remote track record. Would love to connect. |
| 2 | Paul Phillips | GitLab | Talent Acquisition | Hi Paul, came across your Talent Acquisition work at GitLab. I'm a Senior PM based in Argentina, 15+ years building AI-powered products, drawn to GitLab's remote-first culture. Would love to connect. |
| 3 | Florencia Gandulia Nordmann | Deel | Engineer (hiring LatAm roles) | Hi Florencia, saw you're helping grow Deel's LatAm team. I'm a Senior PM (AI/LLM products) based in Argentina -- Deel's whole mission mirrors my own remote work history. Would love to connect. |
| 4 | Katherine LaRue | Nubank | Head of Tech Recruiting | Hi Katherine, saw you lead Tech Recruiting across LatAm at Nubank. I'm a Senior PM based in Argentina with 15+ years in fintech-adjacent, AI-powered products. Would love to connect and learn more. |
| 5 | Daniella Barbosa | Nubank | Talent Acquisition, People & Culture | Hi Daniella, saw your Talent Acquisition work at Nubank. I'm a Senior PM based in Argentina, background spans fintech and AI products. Nubank's LatAm-first model is a strong fit -- would love to connect. |
| 6 | Celina Guajardo | HubSpot | Senior Recruiter | Hi Celina, saw you're growing HubSpot's LatAm team as Senior Recruiter. I'm a Senior PM based in Argentina, 15+ years building AI-powered products across EdTech, fintech and health. Would love to connect. |
| 7 | Yesenia Reyna | HubSpot | Global Recruiter (LatAm) | Hi Yesenia, saw you're hiring for HubSpot's LatAm team. I'm a Senior PM based in Argentina with 15+ years leading AI-powered products for distributed, global teams. Would love to connect. |
| 8 | Maíra Sampaio | VTEX | Talent Acquisition / Tech Recruiter | Hi Maira, saw your Tech Recruiting work at VTEX. I'm a Senior PM based in Argentina, 15+ years building products for LatAm and global distributed teams, now focused on AI-powered products. Would love to connect. |
| 9 | Fernanda Müller | VTEX | Recruiting (Brasil + internacional) | Hi Fernanda, saw you recruit for VTEX both in Brazil and beyond. I'm a Senior PM based in Argentina, background in AI-powered products for distributed LatAm/global teams. Would love to connect. |
| 10 | Michael Orth | Twilio | Sr Manager, Talent Acquisition (NAMER/LATAM) | Hi Michael, saw you lead Talent Acquisition for R&D/G&A across NAMER and LATAM at Twilio. I'm a Senior PM based in Argentina, 15+ years in AI-powered products. Would love to connect. |
| 11 | Daniela Bohórquez | Twilio | Sr Manager, Talent Acquisition (Americas) | Hi Daniela, saw your Talent Acquisition work across the Americas at Twilio. I'm a Senior PM based in Argentina with 15+ years building AI-powered, distributed-team products. Would love to connect. |
| 12 | Camila Uribe | Twilio | Sr Manager, Talent Acquisition (Americas) | Hi Camila, saw your Talent Acquisition role covering the Americas at Twilio. I'm a Senior PM based in Argentina, 15+ years leading AI-powered products for global teams. Would love to connect. |
| 13 | Andrés Miguel Díaz | Zendesk | Talent Partner (México) | Hola Andrés, vi tu rol como Talent Partner en Zendesk. Soy Senior PM basado en Argentina, con 15+ años liderando productos con IA para equipos globales distribuidos. Me encantaría conectar. |
| 14 | Reema Polignano | Anthropic | Technical Recruiter, Infrastructure | Hi Reema, saw you recruit for Anthropic's Infrastructure org. I'm a Senior PM based in Argentina who's shipped LLM/RAG products in production and just finished an AI Master's. Would love to connect. |
| 15 | Marisa Hurtado | Anthropic | Recruiter (ex-Apple, Tesla, Splunk) | Hi Marisa, saw your recruiting work at Anthropic after Apple, Tesla and Splunk. I'm a Senior PM based in Argentina who's built RAG/LLM products in production. Would love to connect. |
| 16 | Gerald H. | GitHub | Sr. Talent Partner | Hi Gerald, saw you're a Talent Partner representing GitHub, a remote-first team. I'm a Senior PM based in Argentina with 15+ years building AI-powered products remotely. Would love to connect. |
| 17 | Eric Coleman | PayPal | Senior Recruiter, Cyber Security (US/LATAM) | Hi Eric, saw you recruit for PayPal's Cyber Security team across the US and LATAM. I'm a Senior PM based in Argentina, background spans fintech and AI-powered products. Would love to connect. |
| 18 | Tim Barnes | Shopify | Lead Recruiter | Hi Tim, saw you're Lead Recruiter at Shopify. I'm a Senior PM based in Argentina, 15+ years building AI-powered products for distributed, global teams. Would love to connect. |

**Nota de shortfall (18 de 25):** no se fuerzan los 7 restantes para completar la cuota. Para Notion, Duolingo, Kavak, Atlassian y Stripe se corrieron búsquedas específicas (`WebSearch`) pero no aparecieron personas verificablemente actuales en la empresa **y** con señal de LatAm/remoto — los resultados eran ex-empleados, perfiles de terceros (agencias de reclutamiento) o empleados sin ubicación confirmable. Completar esas 7 requiere navegación directa de LinkedIn (bloqueada por `WebFetch`) para no arriesgar mensajes a personas equivocadas o inventar contexto que no se puede sostener en una respuesta.

**Empresas deprioritizadas esta ronda:** Amazon, Apple y Google tienen gaps de cobertura (3, 2 y 2 conexiones respectivamente) pero sus roles son mayormente presenciales/híbridos en HQ según `empresas-objetivo.md` — esto choca con el filtro duro "remoto excluyente" de `plan-carrera.md`, así que no se les asignaron solicitudes nuevas esta semana.

**Networking virtual de esta semana (MODO REMOTO):** unirte al Slack de Product School y comentar en 2-3 threads relevantes sobre AI product management. También vale sumarte a la comunidad de Lenny (Lenny's Newsletter/Slack) — foco fuerte en PMs seniors y de IA, buen fit con tu especialización.

---

## Seguimientos (Recién Conectados)

Ninguno. Ninguna fila de `rastreador-conexiones.md` muestra una fecha de "Conectado desde" dentro de las últimas 48 horas (las más recientes son OGHENETEJIRI Atebefia en Amazon, 17 Feb 2026, y Sharik Garzón Terán en Mercado Libre, 19 Nov 2025 — ambas muy anteriores). Además, el tracker registra fecha de conexión pero no distingue "solicitada" vs "conectada" en el tiempo, por lo que no se puede confirmar una aceptación reciente aunque existiera. Sugerencia: al aceptar una conexión nueva, anotar la fecha de aceptación en `rastreador-conexiones.md` para que esta sección pueda funcionar en próximas corridas.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
Ninguno generado esta corrida. La regla que dispara este bloque es "roles postulados en las últimas 48 horas sin referido" — y, según el briefing de Parte 1 de hoy, **el contador de postulaciones formales sigue en cero** desde el inicio del sistema (bloqueo de `WebFetch` impide verificar vacantes reales, ver `2026-09-16-part1-roles.md`). Sin una postulación concreta, no hay rol al cual atar un pedido de referido sin inventar contexto.

### Recordatorios (5+ días, sin respuesta)
Ninguno. No existe `referral-tracker-template.md` en el repo, y `rastreador-conexiones.md` no registra pedidos de referido enviados con fecha — solo conexiones existentes y una lista de candidatos prioritarios sugeridos en la corrida anterior (ver abajo). Sin fecha de envío, no hay base para calcular "5+ días sin respuesta".

### Recomendación de mayor apalancamiento (no es un nudge — es la acción más directa disponible hoy)
`rastreador-conexiones.md` ya identifica 6 conexiones de 1er grado de alta prioridad sin ningún pedido de referido activado todavía: **Elena Yndurain** (Microsoft, Director AI PM), **Virginia Silvero** (Globant, Regional Recruiter Lead), **Melina Ruggeri** (Salesforce, LATAM Recruiting Sr Manager), **Maria Jose Trejo Conde** (Mercado Libre, Talent Acquisition IT regional), **Bernardo Manzella** (Globant, Head of People & Capacity Strategy/AI Studios) y **Pedro Alejandro Santamarina** (Mercado Libre, Sr. Product Development Manager). Correr `/pedir-referido` manualmente para cualquiera de estos 6 sigue siendo, siete semanas seguidas, la acción de mayor conversión disponible en el sistema — más que seguir generando solicitudes de conexión en frío.
