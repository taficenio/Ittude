# Parte 3: Pipeline y Coaching - Martes, 15 de septiembre de 2026

## Gate de Calidad

- `plan-carrera.md`: contiene datos reales (nivel, modalidad remoto-excluyente, mercado objetivo, debilidades, oferta ideal). ✅ Gate superado — se continúa con el resto del briefing.
- `historial-entrevistas.md`: solo placeholders de template (`Total de entrevistas: 0`, log con `[Fecha]` sin completar). Se **salteó** la sección de Coaching de Debilidades de Entrevista — no bloquea el resto del output.
- Fuente de pipeline: **no existe `app-tracker.md`** en el repo (tampoco `biblioteca-contexto/rastrear-postulaciones.md`, el nombre alternativo que usa el propio skill `/rastrear-postulaciones`). Se reconstruyó el resumen del pipeline desde `empresas-objetivo.md`, `rastreador-conexiones.md` y los briefings de hoy (Parte 1 y Parte 2).

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas — confirmado en `briefings/2026-09-15-part1-roles.md` ("Postulaciones enviadas: 0") |
| Referido solicitado | 0 | 6 contactos prioritarios identificados en `rastreador-conexiones.md` (Elena Yndurain, Virginia Silvero, Melina Ruggeri, Maria Jose Trejo Conde, Bernardo Manzella, Pedro Alejandro Santamarina) — ninguno con pedido enviado registrado |
| Entrevista programada | 0 | |
| Entrevistado (esperando resultado) | 0 | |
| Etapa de oferta | 0 | |
| Rechazado esta semana | 0 | |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Nota de confiabilidad del dato:** estos números reflejan lo que está *registrado*, no necesariamente lo que pasó en la realidad — no hay forma de confirmar si el usuario envió algo fuera del sistema sin que quede anotado en un tracker.

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones registradas esta semana (ni en las 6 semanas previas, según Parte 1).

Antes de traducir esto en "postular más rápido", el diagnóstico real es estructural, no de esfuerzo:

1. **`WebFetch` bloqueado 39 días consecutivos** (`EGRESS_BLOCKED`, confirmado de nuevo hoy contra 3 dominios). El gate de calidad de datos del propio sistema exige fecha de publicación + elegibilidad remota LatAm confirmadas en la página real antes de puntuar un rol — sin `WebFetch`, ningún hallazgo de `WebSearch` puede cruzar ese gate, así que `/puntuar-oferta` y `/adaptar-cv` no tienen sobre qué trabajar.
2. **Nada queda marcado como enviado.** De los ~304+ mensajes de networking ya redactados en briefings anteriores, cero están marcados como enviados en `rastreador-conexiones.md` (última actualización: 2026-08-13, 33 días sin cambios). `empresas-objetivo.md` tampoco tiene el campo "Prioridad" completado (última actualización: 2026-08-10, 36 días sin cambios). El sistema puede estar generando trabajo real que el usuario ya usó fuera del OS, pero no hay manera de saberlo sin que se registre.

Por eso la recomendación de hoy no es "postulá 2 ofertas" en el sentido literal (no hay ningún rol que haya cruzado el gate de verificación para puntuar) — es desbloquear las dos vías que **no dependen de `WebFetch`**:

- **Referidos cálidos** (contactos de 1er grado ya identificados, cero necesidad de verificar una vacante externa).
- **Verificación manual de los 2 candidatos de Parte 1** (Rappi "Senior Product Manager I", listings de Bitso) — abrí esos links vos directamente en el navegador, confirmá fecha + elegibilidad remota, y si pasan el gate corré `/puntuar-oferta` con esos datos confirmados a mano.

Si en los próximos días seguís sin poder levantar el bloqueo de `WebFetch`, valdría la pena revisar la configuración de red de la sesión en vez de seguir reintentando los mismos dominios cada día.

---

## Coaching de Persona

### Candidato Remoto
`plan-carrera.md` marca la modalidad remota como filtro duro y excluyente. Parte 1 de hoy no reportó ninguna advertencia de híbrido/presencial en los hallazgos revisados (Rappi y Bitso quedaron sin puntuar por falta de verificación de fecha/elegibilidad, no por modalidad). Parte 2 confirmó que el lote de 25 solicitudes de conexión priorizó empresas remote-friendly (13 de 25, 52%, incluyendo GitLab, Deel, Nubank — remote-first o remoto regional LatAm confirmado). Sin acción adicional requerida hoy en este frente.

*(Career Returner, Director+/Empleado y Founder a Empleado: ninguno aplica según los datos de `plan-carrera.md` — el gap actual es de ~1 mes y ya está reencuadrado como transición normal, no como gap de carrera; no hay indicación de nivel Director+ ni de background de founder/CEO en cargo cerrado.)*

---

## Coaching de Debilidades de Entrevista

Salteado — `historial-entrevistas.md` no tiene entrevistas registradas (0 total). Esta sección se activa automáticamente después de la primera entrevista real vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Activar los 6 referidos cálidos ya identificados.** Correr `/pedir-referido` para al menos 2-3 de: Elena Yndurain (Microsoft), Virginia Silvero (Globant), Melina Ruggeri (Salesforce), Maria Jose Trejo Conde (Mercado Libre), Bernardo Manzella (Globant), Pedro Alejandro Santamarina (Mercado Libre). No dependen de `WebFetch` ni de una vacante puntuada.
2. **Enviar las 25 solicitudes de conexión de `briefings/2026-09-15-part2-networking.md`** desde LinkedIn directamente (verificando visualmente cada perfil primero, ya que no se pudieron abrir con `WebFetch`) — y anotar la fecha de envío por persona en `rastreador-conexiones.md` al terminar. Sin ese registro, este bloque va a seguir vacío en cada corrida futura.
3. **Verificar manualmente los 2 candidatos de Parte 1** (Rappi "Senior Product Manager I", listings de Bitso) abriendo los links vos mismo en el navegador. Si confirmás fecha de publicación + elegibilidad remota LatAm, correr `/puntuar-oferta` con esos datos.
4. **Si hay tiempo:** crear `biblioteca-contexto/rastrear-postulaciones.md` (o `app-tracker.md`) para que el pipeline deje de reconstruirse desde cero cada día, y completar `plantillas/template-rastreador-referidos.md` con los pedidos reales una vez enviados.

Tiempo estimado: 35-45 minutos total (pasos 1-3; el paso 4 es opcional y puede quedar para el fin de semana).

---

## Bloqueos Estructurales Persistentes (para seguimiento)

1. `WebFetch` bloqueado — 39 días consecutivos (`EGRESS_BLOCKED`), confirmado nuevamente hoy.
2. No existe `app-tracker.md` / `rastrear-postulaciones.md` — el pipeline se reconstruye manualmente cada día desde fuentes indirectas.
3. `rastreador-conexiones.md` sin columna de estado ("solicitada" → "conectada") — 33 días sin actualizarse.
4. `empresas-objetivo.md` sin campo "Prioridad" completado — 36 días sin actualizarse.
