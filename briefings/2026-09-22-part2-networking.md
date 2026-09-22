# Parte 2: Networking - Martes, 22 de septiembre de 2026

## Gate de Calidad

`rastreador-conexiones.md`, `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) -- briefing corre completo.

**Detección de función:** Product Manager / Product Owner (Senior IC, Lead/Head, o especialización en IA -- los tres caminos siguen abiertos según `plan-carrera.md`).

**Modo activado: REMOTO.** `plan-carrera.md` marca modalidad remota como filtro duro ("Remoto excluyente"). Se prioriza el 50%+ del lote de solicitudes hacia empresas remote-friendly confirmadas.

**Modo NO activado: Director+/Empleado.** No hay evidencia de nivel Director+ ni de empleo actual (gap de ~1 mes desde fin de contrato en Amplifire, búsqueda activa) -- se usa el lote estándar de 25.

**Modo NO activado: Returner.** El gap de empleo documentado es de ~1 mes (no un gap de carrera de 1+ año) -- no aplica reactivación de red dormida como tratamiento especial de ese modo. Los 6 contactos prioritarios de abajo se tratan igual que ayer, como Tier C (vínculo débil) según la metodología de `/pedir-referido`, no como "returner".

---

## ⚠️ Estado sin cambios desde ayer -- 40 días de bloqueo en solicitudes nuevas

`rastreador-conexiones.md` no se actualizó desde el **2026-08-13** (40 días) y `empresas-objetivo.md` desde el **2026-08-10** (43 días). No hay CSV nuevo, ni perfiles de LinkedIn pegados, ni confirmación de que los 6 mensajes de reconexión del briefing de ayer (2026-09-21) se hayan enviado. Por disciplina anti-fabricación (`CLAUDE.md`, Regla Clave #1), esta corrida **no genera 25 personas nuevas** -- serían inventadas. Repito el plan de asignación y las queries de búsqueda de ayer sin cambios sustantivos (la cobertura real no se movió), y marco explícitamente que este es ya el segundo día consecutivo sin progreso real registrado en esta parte del sistema.

### Empresas gap identificadas (< 4 conexiones en `rastreador-conexiones.md`)

Cobertura actual sin cambios: solo Globant (16), Mercado Libre/Mercado Pago (16) y Microsoft (5) superan el umbral de 4. Las 105 empresas restantes de `empresas-objetivo.md` son gap. Se excluyen del lote Duolingo, Kavak y Naranja X (modalidad híbrida/presencial -- filtro duro de `plan-carrera.md`).

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

Dado el modo remoto: unite a **Product School Slack** y a la **comunidad de Lenny (Lenny's Newsletter community)**, y comentá en 2-3 threads relevantes sobre roles de Product / IA esta semana.

---

## Seguimientos (Recién Conectados)

`rastreador-conexiones.md` sigue sin trackear estados "solicitada -> conectada" y no tuvo ninguna actualización en 40 días. **No hay conexiones nuevas aceptadas en las últimas 48 horas para hacer seguimiento.**

---

## Pedidos de Referido y Recordatorios

No existe un `referral-tracker-template.md` poblado ni un `app-tracker.md` en el repo -- solo `plantillas/template-rastreador-referidos.md`, que sigue siendo un template vacío sin ninguna sección de rol copiada y completada. No hay datos de (a) pedidos de referido enviados hace 5+ días sin respuesta, ni (b) postulaciones de las últimas 48 horas sin referido asociado.

### Nuevos Pedidos de Referido

Los 6 contactos prioritarios de `rastreador-conexiones.md` (sección "Gap de Cobertura") siguen **sin confirmación de envío** -- no hay fecha de contacto registrada para ninguno, ni ayer ni hoy. Repito los mismos 6 mensajes (Tier C: vínculo débil, charla informal de 15 minutos, no pedido de referido directo todavía -- según la metodología de `/pedir-referido`), sin cambios de contenido porque no cambió ningún dato de fondo:

Tratamiento vos/tú: Virginia Silvero, Bernardo Manzella y Pedro Alejandro Santamarina confirmados de Argentina -- se usa "vos". Elena Yndurain (Microsoft), Melina Ruggeri (Salesforce) y María José Trejo Conde (Mercado Libre) sin país confirmado en la biblioteca -- **[VERIFICAR PAÍS]**, se usa "tú" por defecto.

- **Elena Yndurain** -- Director AI Product Management, Microsoft: *"Hola Elena, hace tiempo que estamos conectados en LinkedIn y nunca cruzamos palabra. Vi que lideras AI Product Management en Microsoft -- yo vengo trabajando como AI Product Owner (chatbots con RAG/LLM en producción) y complementé eso con un Master's en IA. Me encantaría escuchar cómo ves el mercado de roles de producto de IA hoy -- ¿tendrías 15 minutos para charlar? Sin ningún pedido puntual, genuina curiosidad por tu perspectiva."*

- **Virginia Silvero** -- Regional Recruiter Lead, South of LatAm, Globant: *"Hola Virginia! Somos conexión de Globant desde hace un tiempo largo y nunca charlamos. Estoy evaluando activamente mi próximo rol de Product (Senior PM / AI Product), 100% remoto. Como liderás reclutamiento regional ahí, me encantaría escuchar tu perspectiva sobre cómo está el mercado de Product en Globant hoy -- ¿tenés 15 minutos para una charla rápida? Sin pedido puntual todavía, solo quiero entender el panorama."*

- **Melina Ruggeri** -- LATAM Recruiting Senior Manager, Salesforce: *"Hola Melina, somos conexión en LinkedIn de hace años y nunca hablamos. Estoy evaluando activamente roles de Product Manager remotos en LatAm, y vi que lideras reclutamiento LATAM en Salesforce. Me encantaría escuchar tu visión de cómo está el mercado de Product ahí -- ¿tendrías 15 minutos para una charla informal? Sin ningún pedido concreto todavía, genuina curiosidad."*

- **Maria Jose Trejo Conde** -- Regional Talent Acquisition IT Senior Analyst, Mercado Libre: *"Hola María José, somos conexión hace años en LinkedIn y nunca cruzamos mensaje. Estoy evaluando activamente mi próximo rol de Product Manager remoto en LatAm, y vi que lideras Talent Acquisition IT regional en Mercado Libre. Me encantaría conocer tu perspectiva sobre cómo está el pipeline de roles de Product ahí -- ¿tendrías 15 minutos para charlar? Ningún pedido puntual todavía, solo quiero entender el panorama."*

- **Bernardo Manzella** -- Head of People & Capacity Strategy (AI Studios), Globant: *"Hola Bernardo! Hace mucho que somos conexión de Globant y nunca hablamos. Vi que liderás People & Capacity Strategy en AI Studios -- justo el cruce entre People y foco en IA que también es mi especialización (Master's en IA + rol de AI Product Owner). Me encantaría escuchar cómo ves el área hoy -- ¿tenés 15 minutos para una charla rápida? Sin pedido concreto, genuina curiosidad por tu perspectiva."*

- **Pedro Alejandro Santamarina** -- Sr. Product Development Manager, Mercado Libre: *"Hola Pedro! Somos conexión de hace años en Mercado Libre/Mercado Pago y nunca charlamos. Estoy evaluando activamente mi próximo rol de Product Manager Senior, remoto, y vi que liderás Product Development ahí. Me encantaría escuchar tu perspectiva sobre cómo es el equipo de Product hoy -- ¿tenés 15 minutos para una charla informal? Sin pedido puntual todavía, solo curiosidad genuina."*

### Recordatorios (5+ días, sin respuesta)

Ninguno -- sin tracker de pedidos de referido enviados, no hay base para generar recordatorios reales.

---

## Resumen accionable de hoy

1. **Bloqueo real, no de research:** correr las 11 queries de LinkedIn de arriba y pegar los resultados es lo único que desbloquea el lote real de 25 solicitudes de conexión nuevas. Esto lleva **40 días** pendiente sin moverse.
2. Enviar los 6 mensajes de reconexión de arriba (Tier C, charla informal) -- también sin confirmación de envío desde que se generaron por primera vez.
3. Unirte a Product School Slack y a la comunidad de Lenny, comentar en 2-3 threads.
4. Después de cualquier envío, actualizar `rastreador-conexiones.md` con fecha y resultado -- sin esto, esta parte del sistema seguirá generando el mismo output día tras día sin poder medir progreso real.
