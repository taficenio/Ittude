# Parte 2: Networking - Lunes, 21 de septiembre de 2026

## Gate de Calidad

`rastreador-conexiones.md`, `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) -- briefing corre completo.

**Detección de función:** Product Manager / Product Owner (Senior IC, Lead/Head, o especialización en IA -- los tres caminos siguen abiertos según `plan-carrera.md`).

**Modo activado: REMOTO.** `plan-carrera.md` marca modalidad remota como filtro duro ("Remoto excluyente"). Se prioriza el 50%+ del lote de solicitudes hacia empresas remote-friendly confirmadas.

**Modo NO activado: Director+/Empleado.** No hay evidencia de nivel Director+ ni de empleo actual (gap de ~1 mes desde fin de contrato en Amplifire, búsqueda activa) -- se usa el lote estándar de 25.

**Modo NO activado: Returner.** El gap de empleo documentado es de ~1 mes (no un gap de carrera de 1+ año) -- no aplica reactivación de red dormida como tratamiento especial. Igual, ver más abajo el punteo de reconexión con los 6 contactos prioritarios: son de la misma naturaleza (red antigua sin interacción reciente), tratados como Tier C según la metodología de `/pedir-referido`.

---

## ⚠️ Bloqueo en Solicitudes de Conexión Nuevas -- explicación

Según `.claude/skills/solicitud-conexion/SKILL.md`, generar los 25 mensajes de solicitud de conexión requiere perfiles reales de LinkedIn (nombre, rol, actividad reciente) para cada gap company, porque Claude no puede buscar en LinkedIn directamente. Esta sesión no tiene acceso a LinkedIn ni recibió ningún input de perfiles nuevos (no hay CSV ni pegado de resultados de búsqueda en este run automatizado).

**No se fabricaron 25 personas ficticias** -- inventar nombres y roles de gente real que podría no existir viola la regla más importante del sistema (nunca fabricar; ver `CLAUDE.md`, sección Reglas Clave #1) y podría hacerte enviar solicitudes a perfiles que no existen o mal identificados.

En su lugar, abajo va el **plan de asignación round-robin ya armado** (a qué empresas, cuántas personas cada una, con prioridad remote-first) y **las queries de búsqueda de LinkedIn exactas** para cada empresa. Corré las búsquedas, pegá los resultados (nombre + rol + últimos posts si tienen), y el siguiente `/solicitud-conexion` genera los 25 mensajes reales con esos datos.

### Empresas gap identificadas (< 4 conexiones en `rastreador-conexiones.md`)

Cobertura actual: solo Globant (16), Mercado Libre/Mercado Pago (16) y Microsoft (5) superan el umbral de 4. Las 105 empresas restantes de `empresas-objetivo.md` son gap. Se descartan del lote de hoy Duolingo, Kavak y Naranja X (modalidad híbrida/presencial -- filtro duro de `plan-carrera.md`, ver notas en `2026-09-21-part1-roles.md` y en `rastreador-conexiones.md`).

### Plan de asignación (25 solicitudes, round-robin, 11 empresas)

**Bloque remote-first confirmado (13 de 25 -- cumple el mínimo 50% de MODO REMOTO):**

| Empresa | Cupo | Señal remote-first (fuente: `empresas-objetivo.md`) |
|---|---|---|
| GitLab | 3 | "100% remota desde su fundación (sin oficinas)" |
| Deel | 3 | "Privada (decacornio), full-remote" |
| Atlassian | 3 | "cultura remote-first" |
| Shopify | 2 | "remote-first declarado" |
| Remote.com | 2 | "misma lógica de afinidad que Deel" (EOR global) |

**Bloque resto de Tier 1 (12 de 25):**

| Empresa | Cupo |
|---|---|
| Nubank | 2 |
| Anthropic | 2 |
| Stripe | 2 |
| HubSpot | 2 |
| Notion | 2 |
| VTEX | 2 |

### Queries de búsqueda para pegar resultados

Para cada empresa, necesito 1-2 PM a tu nivel, 1 PM un nivel arriba (Director/Group PM), 1 función adyacente (Eng Manager / Design Lead), y 1 wildcard (reclutador o alguien activo en LinkedIn) -- según el mix de `/solicitud-conexion`.

```
LinkedIn search: "GitLab" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Deel" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Atlassian" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Shopify" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Remote.com" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Nubank" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Anthropic" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Stripe" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "HubSpot" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "Notion" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
LinkedIn search: "VTEX" AND ("Product Manager" OR "Group Product Manager" OR "Engineering Manager")
```

Para cada persona, anotá si tiene posts recientes o algún punto de conexión (misma escuela, ex-empleador compartido, ciudad) -- eso es lo que hace que el mensaje no sea genérico.

### Networking virtual de esta semana

Dado el modo remoto: unite a **Product School Slack** y a la **comunidad de Lenny (Lenny's Newsletter community)**, y comentá en 2-3 threads relevantes sobre roles de Product / IA esta semana. Esto genera señal orgánica sin depender de solicitudes en frío.

---

## Seguimientos (Recién Conectados)

`rastreador-conexiones.md` no trackea estados "solicitada -> conectada" -- todas las entradas actuales son conexiones de 1er grado ya establecidas (importadas del CSV de LinkedIn), sin fecha de aceptación reciente registrada. **No hay conexiones nuevas aceptadas en las últimas 48 horas para hacer seguimiento.** Esto se resolverá automáticamente una vez que empiecen a aceptarse las solicitudes del plan de arriba -- `rastreador-conexiones.md` se actualiza post-envío según el comportamiento automático #4 de `CLAUDE.md`.

---

## Pedidos de Referido y Recordatorios

**No existe `referral-tracker-template.md` ni un `app-tracker.md` en el repo** -- no hay datos de (a) pedidos de referido enviados hace 5+ días sin respuesta, ni (b) postulaciones de las últimas 48 horas sin referido asociado. Ambas sub-secciones del formato estándar quedan vacías por falta de tracker, no por falta de trabajo.

### Nuevos Pedidos de Referido

Lo que sí hay: la nota de "Gap de Cobertura" al final de `rastreador-conexiones.md` señala 6 contactos de alta prioridad, identificados hace 39 días, **ninguno contactado todavía** (confirmado en `2026-09-21-part1-roles.md`). Para los 6, `rastreador-conexiones.md` no registra ninguna interacción más allá de la fecha de conexión original en LinkedIn (todas de 2010-2021) -- por la metodología de `/pedir-referido` (clasificación de fuerza de vínculo), esto los pone en **Tier C: vínculo débil**. Según esa metodología, no corresponde pedir referido directo todavía -- corresponde una charla informal de 15 minutos primero. Los mensajes de abajo siguen ese formato, no el de pedido de referido directo.

Tratamiento vos/tú: Virginia Silvero, Bernardo Manzella y Pedro Alejandro Santamarina están confirmados como contactos de Argentina (ver notas de Globant/Mercado Libre en `rastreador-conexiones.md`) -- se usa "vos". Elena Yndurain (Microsoft) y Melina Ruggeri (Salesforce) no tienen país confirmado en la biblioteca -- **[VERIFICAR PAÍS]**, se usa "tú" por defecto hasta confirmar. Para María José Trejo Conde (Mercado Libre), la nota de la empresa dice "mayormente Argentina" pero no confirma su caso puntual -- **[VERIFICAR PAÍS]**, mismo criterio de "tú" por defecto.

- **Elena Yndurain** -- Director AI Product Management, Microsoft: *"Hola Elena, hace tiempo que estamos conectados en LinkedIn y nunca cruzamos palabra. Vi que lideras AI Product Management en Microsoft -- yo vengo trabajando como AI Product Owner (chatbots con RAG/LLM en producción) y complementé eso con un Master's en IA. Me encantaría escuchar cómo ves el mercado de roles de producto de IA hoy -- ¿tendrías 15 minutos para charlar? Sin ningún pedido puntual, genuina curiosidad por tu perspectiva."*

- **Virginia Silvero** -- Regional Recruiter Lead, South of LatAm, Globant: *"Hola Virginia! Somos conexión de Globant desde hace un tiempo largo y nunca charlamos. Estoy evaluando activamente mi próximo rol de Product (Senior PM / AI Product), 100% remoto. Como liderás reclutamiento regional ahí, me encantaría escuchar tu perspectiva sobre cómo está el mercado de Product en Globant hoy -- ¿tenés 15 minutos para una charla rápida? Sin pedido puntual todavía, solo quiero entender el panorama."*

- **Melina Ruggeri** -- LATAM Recruiting Senior Manager, Salesforce: *"Hola Melina, somos conexión en LinkedIn de hace años y nunca hablamos. Estoy evaluando activamente roles de Product Manager remotos en LatAm, y vi que lideras reclutamiento LATAM en Salesforce. Me encantaría escuchar tu visión de cómo está el mercado de Product ahí -- ¿tendrías 15 minutos para una charla informal? Sin ningún pedido concreto todavía, genuina curiosidad."*

- **Maria Jose Trejo Conde** -- Regional Talent Acquisition IT Senior Analyst, Mercado Libre: *"Hola María José, somos conexión hace años en LinkedIn y nunca cruzamos mensaje. Estoy evaluando activamente mi próximo rol de Product Manager remoto en LatAm, y vi que lideras Talent Acquisition IT regional en Mercado Libre. Me encantaría conocer tu perspectiva sobre cómo está el pipeline de roles de Product ahí -- ¿tendrías 15 minutos para charlar? Ningún pedido puntual todavía, solo quiero entender el panorama."*

- **Bernardo Manzella** -- Head of People & Capacity Strategy (AI Studios), Globant: *"Hola Bernardo! Hace mucho que somos conexión de Globant y nunca hablamos. Vi que liderás People & Capacity Strategy en AI Studios -- justo el cruce entre People y foco en IA que también es mi especialización (Master's en IA + rol de AI Product Owner). Me encantaría escuchar cómo ves el área hoy -- ¿tenés 15 minutos para una charla rápida? Sin pedido concreto, genuina curiosidad por tu perspectiva."*

- **Pedro Alejandro Santamarina** -- Sr. Product Development Manager, Mercado Libre: *"Hola Pedro! Somos conexión de hace años en Mercado Libre/Mercado Pago y nunca charlamos. Estoy evaluando activamente mi próximo rol de Product Manager Senior, remoto, y vi que liderás Product Development ahí. Me encantaría escuchar tu perspectiva sobre cómo es el equipo de Product hoy -- ¿tenés 15 minutos para una charla informal? Sin pedido puntual todavía, solo curiosidad genuina."*

### Recordatorios (5+ días, sin respuesta)

Ninguno -- sin tracker de pedidos de referido enviados, no hay base para generar recordatorios reales. Una vez que se envíen los 6 mensajes de arriba y se registren en `rastreador-conexiones.md` con fecha, este briefing podrá generar recordatorios automáticamente a partir del día 6.

---

## Resumen accionable de hoy

1. Correr las 11 queries de LinkedIn de arriba y pegar los resultados para desbloquear el lote real de 25 solicitudes de conexión nuevas.
2. Enviar los 6 mensajes de reconexión de arriba (Tier C, charla informal -- no referido directo todavía).
3. Unirte a Product School Slack y a la comunidad de Lenny, comentar en 2-3 threads.
4. Después de cualquier envío, actualizar `rastreador-conexiones.md` con fecha y resultado -- esto es lo que va a permitir que las próximas corridas de Parte 2 generen seguimientos y recordatorios reales en vez de secciones vacías.
