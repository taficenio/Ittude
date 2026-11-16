# Parte 2: Networking - Lunes, 16 de Noviembre de 2026

## Nota de Transparencia (leer antes del resto)

Este briefing corrió de forma desatendida (Parte 2 de 3). Gate de calidad antes de generar nada:

- `empresas-objetivo.md`, `plan-carrera.md` y `rastreador-conexiones.md` tienen datos reales (no placeholders de template) — el gate pasa, se continúa.
- **Modo detectado: REMOTO.** `plan-carrera.md` marca "Remoto excluyente" como filtro duro. Aplican las reglas de modo remoto abajo.
- **Modo Director+/Empleado: no aplica.** El usuario no está empleado actualmente (el contrato en Amplifire terminó hace ~1 mes, ver `plan-carrera.md`) y el plan de carrera no fija Director+ como objetivo único — son 3 caminos abiertos (IC Senior, Lead/Head, especialización IA).
- **Modo Returner: no aplica.** El único "gap" documentado en `plan-carrera.md` es de ~1 mes entre el fin de Amplifire y hoy, explícitamente marcado como transición normal que no necesita guión de reactivación. No es el escenario de gap de carrera extendido que dispara este modo.
- **Limitación real de datos, sin cambios desde la corrida del 2026-11-13:** `rastreador-conexiones.md` sigue sin actualizarse desde el 2026-08-13 — **95 días sin tocar** (mismo número que señala hoy `briefings/2026-11-16-part1-roles.md`). Solo contiene conexiones de **1er grado ya existentes** importadas de un export de LinkedIn. No hay ninguna fuente en este repo con nombres reales de personas de 2do/3er grado en las ~99 empresas objetivo sin cobertura. Generar 25 "solicitudes de conexión" a personas inventadas violaría la regla central del sistema (nunca fabricar — ver `CLAUDE.md`) y enviaría invitaciones reales de LinkedIn a perfiles que no existen. Por eso esta corrida, igual que la del viernes pasado, prioriza valor real y verificable sobre volumen: **6 mensajes de reactivación a personas reales** en empresas con gap de cobertura, en vez de 25 genéricos, más una lista concreta de búsqueda manual para el resto.

---

## Solicitudes de Conexión — Reactivación Prioritaria (6 contactos reales, empresas con gap de cobertura)

Empresas objetivo con menos de 4 conexiones de 1er grado, con contactos reales disponibles en `rastreador-conexiones.md`. Ya son conexiones de 1er grado, así que no son "solicitudes" de LinkedIn sino mensajes de reactivación — pero cumplen la misma función: abrir la puerta en empresas con gap. (Se excluyen de esta lista Sophia Malik — Amazon, rol no relacionado a producto — y Esther Sack — Salesforce, es partner no empleada — por baja relevancia, ya señalado en `rastreador-conexiones.md`.)

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Alejandro Medici | Amazon (AWS) | Startup Solution Architect | Hola Alejandro, ¡hace mucho no hablamos! Conectamos en 2013. Ando buscando mi próximo rol como PM Senior (fintech, EdTech, IA) y Amazon/AWS está en mi radar. ¿Tenés 15 min para contarme cómo ves hoy el área de producto? |
| 2 | OGHENETEJIRI Atebefia | Amazon (AWS) | Security Operations Center Analyst | Hi Oghenetejiri, great to connect on AWS! I'm exploring my next Senior PM role (15+ years across EdTech, fintech, AI). Would love to hear how you're finding the Security Ops side there — got 15 min for a quick chat? |
| 3 | Pablo Perez | Apple | AIML | Hola Pablo, ¡cuánto tiempo! Conectamos en 2019. Hoy busco mi próximo rol como PM Senior con foco en IA (vengo de liderar RAG/LLM en Amplifire) y tu trabajo en AIML en Apple me interesa mucho. ¿Tenés 15 min para charlar? |
| 4 | jason cohen | Apple | Sr Technical Recruiter, Silicon Engineering Group | Hi Jason, it's been a while — we connected back in 2013! I'm actively exploring my next Senior PM role (15+ years in EdTech, fintech, AI). Given your recruiting work at Apple, would you have 15 min to share any product-side openings? |
| 5 | Gabriel Sleiman | Google | Infrastructure Cloud Engineer | Hola Gabriel, hace tiempo que conectamos (2019). Estoy buscando mi próximo rol como PM Senior (fintech, EdTech, IA) y Google está en mi radar. ¿Tendrías 15 minutos para contarme cómo ves el área de producto desde tu rol? |
| 6 | Carlos Amilcar Sanchez Rosa | Atlassian | Senior Software Engineer | Hola Carlos, ¡cuánto tiempo! Conectamos en 2021. Estoy explorando mi próximo rol como PM Senior (uso Jira/Confluence hace años) y Atlassian es de mis empresas objetivo — 100% remote-first, justo lo que busco. ¿15 min para charlar? |

*(Cristian Devrient en Google queda como opción de reserva si estos 6 no responden en la primera semana — ver `rastreador-conexiones.md`.)*

## Gap Real de Cobertura — Requiere Búsqueda Manual en LinkedIn

Las empresas Tier 1/Tier 2 con **0 conexiones de 1er grado** no tienen ningún nombre real disponible en este sistema. No se inventaron. Lista priorizada para búsqueda manual esta semana:

**Prioridad 1 — Acción crítica (modo remoto, confirmada remote-friendly, y ya hay trabajo hecho esperando):**
- **Deel** — full-remote, infraestructura de contratación remota global. Es el lead más caliente del sistema: dos CVs ya generados y verificados (Senior PM FinTech 80/100, Staff PM Time & Workforce 79/100) llevan 40 y 43 días esperando sin un contacto interno que empuje. Buscar "Recruiter LATAM Deel" o "Product Manager Deel" en LinkedIn, filtrar 2do grado, pedir conexión personalizada.
- **GitLab** — 100% remota desde su fundación.
- **Atlassian, Shopify** (remote-first confirmado en `empresas-objetivo.md`), más Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub, Remote.com (SaaS remoto-friendly / infraestructura remota confirmada).

**Prioridad 2 — Tier 1 sin conexión, remoto regional LatAm confirmado:**
- Nubank, VTEX (también tiene CV verificado 72/100 esperando ~74 días), Kavak.

**Prioridad 3 — Tier 1 sin conexión, remoto a verificar caso por caso:**
- Stripe, HubSpot, Notion, Duolingo, Anthropic.

Búsqueda sugerida por empresa: "Recruiter LATAM [empresa]" o "Product Manager [empresa]" en LinkedIn → filtrar por 2do grado → pedir conexión con mensaje personalizado (<300 caracteres) una vez identificada una persona real.

## Networking Virtual de Esta Semana (modo remoto)

Unirte a la comunidad de **Lenny's Newsletter** (Lenny Rachitsky, PMs) y comentar en 2-3 threads relevantes. Alternativa: **Product School Slack**. Ambas tienen canales activos de referidos internos para roles remotos.

---

## Seguimientos (Recién Conectados)

Ninguno. `rastreador-conexiones.md` no registra ninguna transición de "solicitada" a "conectada" en las últimas 48 horas — de hecho no registra ningún cambio desde el 2026-08-13 (95 días). No hay base para generar seguimientos hoy.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)
Ninguno. `template-rastreador-referidos.md` sigue siendo el template vacío — ningún pedido de referido fue registrado como enviado todavía, así que no hay nada que recordar.

### Nuevos Pedidos de Referido
Los 6 contactos de mayor prioridad de `rastreador-conexiones.md` siguen sin un primer contacto, **95 días después de haberse identificado** — el mismo bloqueo que señala `part1-roles.md` hoy. Ninguno tiene hoy un rol remoto confirmado al cual anclar el pedido: la investigación de hoy descartó o dejó sin verificar los postings de Globant, Salesforce, Mercado Libre y Microsoft (ver `briefings/2026-11-16-part1-roles.md`), así que estos mensajes son de reconexión/exploración general, no un pedido de referido atado a una vacante específica — consistente con la filosofía de "conversación primero, pedido puntual después".

- **Virginia Silvero** (Globant, Regional Recruiter Lead South of LatAm): "Hola Virginia! Hace tiempo no hablamos — conectamos en 2010. Hoy estoy buscando mi próximo rol como PM Senior (15+ años en EdTech, fintech y salud, con foco reciente en IA). ¿Tendrías 15 minutos para contarme cómo está hoy el área de producto en Globant y si ves algún fit?"
- **Bernardo Manzella** (Globant, Head of People & Capacity Strategy, AI Studios): "Hola Bernardo! Conectamos hace años en Globant. Estoy evaluando roles de PM Senior con foco en IA (lideré un proyecto de chatbot con RAG/LLM en Amplifire). Dado tu rol en AI Studios, ¿tendrías 15 min para una charla y contarme si hay espacio para un perfil como el mío?"
- **Melina Ruggeri** (Salesforce, LATAM Recruiting Senior Manager): "Hola Melina! Hace un tiempo que no hablamos — conectamos en 2017. Estoy buscando activamente mi próximo rol como PM Senior (15+ años en EdTech, fintech y salud) y Salesforce siempre estuvo en mi radar. ¿Tenés 15 minutos para contarme cómo está el equipo de producto hoy?"
- **Maria Jose Trejo Conde** (Mercado Libre, Regional Talent Acquisition IT Senior Analyst): "Hola María José, ¿cómo estás? Nos conectamos hace unos años. Estoy explorando roles de PM Senior (15+ años en EdTech, fintech y salud) y Mercado Libre está entre mis empresas objetivo. ¿Tendrías 15 minutos para platicar sobre el área de producto?"
- **Elena Yndurain** (Microsoft, Director AI Product Management): "Hola Elena, espero que estés muy bien. Nos conectamos en 2021. Vi tu rol liderando AI Product Management en Microsoft y me pareció muy relevante: vengo de liderar un proyecto de chatbot con RAG/LLM en Amplifire y hoy busco mi próximo rol como PM Senior con foco en IA. ¿15 minutos para charlar?"
- **Pedro Alejandro Santamarina** (Mercado Libre, Sr. Product Development Manager): "Hola Pedro! Hace tiempo no hablamos — conectamos en 2013. Hoy estoy buscando mi próximo rol como PM Senior (15+ años en EdTech, fintech y salud). Dado tu rol en Product, ¿tendrías 15 minutos para contarme cómo ves el área hoy?"

### Roles postulados en las últimas 48 horas sin referido
Ninguno — `part1-roles.md` confirma 0 postulaciones enviadas en total hasta la fecha. No aplica esta sección hoy.

---

## Resumen de Acción para Hoy

1. Enviar los 6 mensajes de reactivación prioritaria (empresas con gap real y contacto real disponible).
2. Enviar los 6 pedidos de referido/reconexión de mayor prioridad — 95 días identificados sin contacto, el mismo número que viene marcando el sistema desde el viernes.
3. Esta semana: unirte a la comunidad de Lenny y comentar en 2-3 threads.
4. Más urgente que cualquier solicitud nueva: buscar manualmente 1 persona real en Deel (full-remote, 2 CVs esperando 40-43 días) y activar esa conexión — es la brecha de mayor apalancamiento del sistema hoy.
5. Pendiente de criterio propio (no automatizable sin fabricar datos): completar la búsqueda manual en GitLab, Atlassian, Shopify y el resto de la lista de "Gap Real de Cobertura", priorizando remote-friendly para cumplir el objetivo de modo remoto (50%+ del outreach).
