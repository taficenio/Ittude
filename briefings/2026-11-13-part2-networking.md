# Parte 2: Networking - Viernes, 13 de Noviembre de 2026

## Nota de Transparencia (leer antes del resto)

Este briefing corrió de forma desatendida. Antes de generar solicitudes de conexión, confirmo lo siguiente:

- `empresas-objetivo.md`, `plan-carrera.md` y `rastreador-conexiones.md` tienen datos reales (no placeholders) — el gate de calidad pasa.
- **Modo detectado:** REMOTO (plan-carrera.md: "Remoto excluyente"). No aplica modo Director+/Empleado (el usuario no está empleado actualmente — el contrato en Amplifire terminó hace ~1 mes, ver `plan-carrera.md`). No aplica modo Returner (el gap de empleo es de ~1 mes, explícitamente documentado como que no necesita estrategia de reactivación de red).
- **Limitación real de datos — importante:** `rastreador-conexiones.md` contiene únicamente conexiones de **1er grado ya existentes** (importadas desde un export de LinkedIn el 2026-08-13, sin actualizar desde entonces). No hay ninguna fuente en este repo con nombres reales de personas de 2do/3er grado en las empresas objetivo sin cobertura. Generar 25 "solicitudes de conexión" a personas inventadas violaría la regla central del sistema (nunca fabricar — ver `CLAUDE.md`), y además sería enviar invitaciones reales de LinkedIn a perfiles que no existen. Por eso esta corrida prioriza valor real y verificable: **12 mensajes a personas reales ya identificadas** (de reconexión y de pedido de referido) en vez de 25 genéricos, y una lista concreta de búsqueda manual para el resto del gap.

---

## Solicitudes de Conexión — Reconexión Prioritaria (6 contactos reales, empresas con gap de cobertura)

Empresas objetivo con menos de 4 conexiones de 1er grado, con contactos reales disponibles en `rastreador-conexiones.md`. Como ya son conexiones de 1er grado, no son "solicitudes" de LinkedIn sino mensajes directos de reactivación — pero cumplen la misma función: activar red en empresas con gap.

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | Alejandro Medici | Amazon (AWS) | Startup Solution Architect | Hola Alejandro, ¡hace mucho no hablamos! Conectamos en 2013. Hoy busco mi próximo rol como Senior PM (fintech, EdTech, IA) y Amazon/AWS está en mi radar. ¿Tenés 15 min para contarme cómo ves el área de producto hoy? |
| 2 | OGHENETEJIRI Atebefia | Amazon (AWS) | Security Operations Center Analyst | Hi Oghenetejiri, great connecting on AWS! I'm exploring my next Senior PM role (15+ years in EdTech, fintech, AI). Would love to hear how you're finding the Security Ops team there — got 15 min for a quick chat? |
| 3 | Pablo Perez | Apple | AIML | Hola Pablo, ¡cuánto tiempo! Nos conectamos en 2019. Hoy busco mi próximo rol como Senior PM con foco en IA (vengo de liderar RAG/LLM en Amplifire) y tu rol en AIML en Apple me interesa mucho. ¿15 minutos para charlar? |
| 4 | jason cohen | Apple | Sr Technical Recruiter, Silicon Engineering Group | Hi Jason, it's been a while since we connected in 2013! I'm actively exploring my next Senior PM role (15+ years in EdTech, fintech, AI). Given your recruiting work at Apple, would you have 15 min to share any product-side openings? |
| 5 | Gabriel Sleiman | Google | Infrastructure Cloud Engineer | Hola Gabriel, hace tiempo conectamos (2019). Hoy estoy buscando mi próximo rol como Senior PM (fintech, EdTech, IA) y Google está en mi radar. ¿Tendrías 15 minutos para contarme cómo ves el área de producto desde tu rol? |
| 6 | Carlos Amilcar Sanchez Rosa | Atlassian | Senior Software Engineer | Hola Carlos, ¡cuánto tiempo! Conectamos en 2021. Hoy estoy explorando mi próximo rol como Senior PM (uso Jira/Confluence hace años) y Atlassian es una de mis empresas objetivo. ¿Tendrías 15 min para charlar? |

*(Cristian Devrient en Google y Esther Sack en Salesforce también están disponibles como opciones de reserva si estos 6 no responden — ver `rastreador-conexiones.md`.)*

## Gap Real de Cobertura — Requiere Búsqueda Manual en LinkedIn

Las empresas Tier 1/Tier 2 con **0 conexiones de 1er grado** no tienen ningún nombre real disponible en este sistema. Generarlos habría significado inventar personas — no lo hice. Lista priorizada para que el usuario busque manualmente en LinkedIn (reclutador regional, hiring manager de Producto, o par senior de Producto) esta semana:

**Prioridad 1 — Remote-friendly confirmadas (modo remoto: asignar al menos el 50% del esfuerzo de outreach acá, algo que esta corrida no pudo cumplir por falta de nombres reales):**
- GitLab (100% remota desde su fundación)
- Deel (full-remote, infraestructura de contratación remota global)
- Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub (SaaS remoto-friendly confirmado en `empresas-objetivo.md`)

**Prioridad 2 — Tier 1 sin conexión, remoto regional confirmado:**
- Nubank, VTEX, Kavak (remoto regional LatAm)

**Prioridad 3 — Tier 1 sin conexión, remoto a verificar:**
- Stripe, HubSpot, Notion, Duolingo, Anthropic

Búsqueda sugerida por empresa: "Recruiter LATAM [empresa]" o "Product Manager [empresa]" en LinkedIn → filtrar por 2do grado → pedir conexión con mensaje personalizado (<300 caracteres) una vez identificada una persona real.

## Networking Virtual de Esta Semana (modo remoto)

Unirte a **Lenny's Newsletter community** (comunidad de Lenny Rachitsky para PMs) y comentar en 2-3 threads relevantes esta semana. Alternativa: **Product School Slack**. Ambas son espacios activos para PMs remotos y suelen tener canales de referidos internos.

---

## Seguimientos (Recién Conectados)

No se encontraron conexiones que pasaran de "solicitada" a "conectada" en las últimas 48 horas. `rastreador-conexiones.md` no registra fechas de solicitud/aceptación recientes — su última actualización real es del 2026-08-13 (92 días sin tocar, según ya señalado en `briefings/2026-11-13-part1-roles.md`). No hay base para generar seguimientos de esta sección hoy.

---

## Pedidos de Referido y Recordatorios

### Recordatorios (5+ días, sin respuesta)
Ninguno. No existe ningún pedido de referido previamente enviado registrado — ni en `rastreador-conexiones.md` ni en `plantillas/template-rastreador-referidos.md` (este último sigue siendo el template vacío, sin ninguna sección completada). No hay nada que recordar todavía.

### Nuevos Pedidos de Referido
Los 6 contactos de mayor prioridad ya identificados en `rastreador-conexiones.md` (sección "Gap de Cobertura") siguen sin un primer contacto, 92 días después de haber sido señalados. Dos de ellos (Globant) tienen un rol concreto para referenciar — el posting recurrente "Product Manager Senior-Level" (Buenos Aires, remoto) que `part1-roles.md` viene registrando desde hace semanas. Los otros cuatro no tienen un rol confirmado hoy, así que el mensaje es de reconexión/exploración, no un pedido de referido formal para un puesto específico — más alineado con la filosofía de "referidos antes que postulaciones frías": primero la conversación, después el pedido puntual.

- **Virginia Silvero** (Globant, Regional Recruiter Lead South of LatAm): "Hola Virginia! Hace tiempo no hablamos — conectamos en 2010 cuando yo estaba en Buenos Aires. Hoy estoy buscando mi próximo rol como PM Senior (15+ años en EdTech, fintech y salud, últimamente con foco en IA) y vi que Globant tiene abierta la posición de Product Manager Senior-Level (remoto, BA). ¿Podrías orientarme sobre el proceso o conectarme con quien lidera la búsqueda? ¡Gracias!"
- **Bernardo Manzella** (Globant, Head of People & Capacity Strategy, AI Studios): "Hola Bernardo! Conectamos hace años en Globant. Hoy estoy evaluando roles de Product Manager Senior con foco en IA (vengo de liderar un proyecto de chatbot con RAG/LLM en Amplifire) y vi que Globant tiene abierta una búsqueda de PM Senior-Level remota en BA. Dado tu rol en AI Studios, ¿te parece que tenga sentido explorarlo? Te agradezco cualquier orientación."
- **Melina Ruggeri** (Salesforce, LATAM Recruiting Senior Manager): "Hola Melina! Hace un tiempo que no hablamos — nos conectamos por LinkedIn en 2017. Estoy buscando activamente mi próximo rol como Senior PM (15+ años en EdTech, fintech y salud) y Salesforce siempre estuvo en mi radar. ¿Tenés 15 minutos para contarme cómo está el equipo de producto hoy y si ves fit para alguien con mi perfil? ¡Gracias de antemano!"
- **Maria Jose Trejo Conde** (Mercado Libre, Regional Talent Acquisition IT Senior Analyst): "Hola María José, ¿cómo estás? Nos conectamos hace unos años. Ahora estoy explorando roles de Senior Product Manager (15+ años en EdTech, fintech y salud, con foco reciente en IA) y Mercado Libre/Mercado Pago está entre mis empresas objetivo. ¿Tendrías 15 minutos para platicar sobre cómo está el área de producto y si ves algún fit? Te lo agradecería mucho."
- **Elena Yndurain** (Microsoft, Director AI Product Management): "Hola Elena, espero que estés muy bien. Soy Ramon — nos conectamos en 2021. Vi tu rol liderando AI Product Management en Microsoft y me pareció una conexión muy relevante: vengo de liderar un proyecto de chatbot con RAG/LLM en Amplifire y hoy busco mi próximo rol como Senior PM con foco en IA. ¿Tendrías 15 minutos para una charla breve? Me encantaría conocer tu perspectiva."
- **Pedro Alejandro Santamarina** (Mercado Libre, Sr. Product Development Manager): "Hola Pedro! Hace tiempo no hablamos — conectamos en 2013. Hoy estoy buscando mi próximo rol como PM Senior (15+ años en EdTech, fintech y salud) y Mercado Libre es una de mis empresas objetivo. Dado tu rol en Product, ¿tendrías 15 minutos para contarme cómo ves el área hoy? Gracias de antemano."

### Roles postulados en las últimas 48 horas sin referido
Ninguno — `part1-roles.md` confirma 0 postulaciones enviadas en total hasta la fecha. No aplica esta sección hoy.

---

## Resumen de Acción para Hoy

1. Enviar los 6 mensajes de reconexión prioritaria (empresas con gap real y contacto real disponible).
2. Enviar los 6 pedidos de referido/reconexión de la lista de mayor prioridad — son los más atrasados del sistema (92 días identificados sin contacto).
3. Esta semana: unirte a la comunidad de Lenny y comentar en 2-3 threads.
4. Pendiente de criterio propio (no automatizable sin fabricar datos): buscar manualmente en LinkedIn 1-2 personas reales por empresa en la lista de "Gap Real de Cobertura", empezando por las remote-friendly (GitLab, Deel, Shopify, Zoom, Twilio, Vercel, Zendesk, Monday.com, Linear, Figma, GitHub) para cumplir el objetivo de modo remoto de 50%+ del outreach en empresas remote-friendly.
