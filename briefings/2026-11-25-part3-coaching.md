# Parte 3: Pipeline y Coaching - Miércoles, 25 de Noviembre de 2026

## Resumen del Pipeline

**Fuente:** No existe `app-tracker.md` en el repo. Armado desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y los briefings de hoy (Parte 1 y Parte 2). Ninguno de estos archivos tiene campos de "Estado de postulación" poblados por postulación individual — los números de abajo reflejan lo que hay registrado, no necesariamente todo lo que pasó en la realidad (ver nota de confiabilidad al final).

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas en ningún archivo de contexto |
| Referido solicitado | 0 | Sin pedidos de referido registrados como enviados |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | — |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Contexto crítico que la tabla no captura:** hay 3 CVs ya generados y verificados con score ≥70/100 — Deel Senior PM FinTech Payments/Credit Control & Risk (80/100, 49 días esperando desde que se generó), Deel Staff PM Time & Workforce Management (79/100, 52 días esperando), VTEX Order Management (72/100, 83 días esperando) — ninguno con evidencia de haber sido enviado. El sistema lleva 108 días corriendo (desde 2026-08-10) con 0 postulaciones enviadas.

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones enviadas esta semana — ni en ninguna semana desde que arrancó el sistema (108 días). A diferencia del escenario genérico de "cero volumen", en este caso **sí hay roles 70+ ya generados y verificados** (los 3 CVs de Deel/VTEX listados arriba), así que la acción no es expandir la lista de targets ni ajustar criteria en `plan-carrera.md` — es simplemente enviar lo que ya existe. Enviar al menos 2 hoy (las dos de Deel, que son las de mayor score).

Un segundo cuello de botella paralelo, documentado en la Parte 2 de hoy: `rastreador-conexiones.md` lleva 104 días sin actualizarse y 6 contactos de referido de alta prioridad (Elena Yndurain - Microsoft, Virginia Silvero y Bernardo Manzella - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde y Pedro Alejandro Santamarina - Mercado Libre) siguen sin activarse desde que se identificaron. Dado que 0 postulaciones implica que el trigger automático de referidos nunca se dispara, esto refuerza el mismo problema: lo generado no se está ejecutando.

## Coaching de Persona

**Persona detectada:** Candidato Remoto (modalidad remota excluyente, confirmado en `plan-carrera.md` como filtro duro). No aplica Career Returner (gap real de ~1 mes, no un gap de carrera), no aplica Director+/Empleado (usuario no está empleado actualmente), no aplica Founder a Empleado, no aplica ritmo de carrera temprana (15+ años de experiencia documentados en `biblioteca-experiencias.md`).

**Revisión cruzada con el escaneo de roles de Parte 1:** se confirman advertencias de modalidad no-remota en varios de los hallazgos revisados hoy — Kavak ("AI Product Manager" en Buenos Aires, descrito como híbrido: 3 días en casa / resto oficina) y Nubank (Senior Staff PM Crypto, marcado "hybrid" por un agregador). Ambos quedaron correctamente descartados en Parte 1 sin llegar a puntuarse, consistente con el filtro duro de modalidad remota de `plan-carrera.md`. El posting de GitLab ("Product Manager, AI Editor Extensions", tag "Remote, Americas; Remote, EMEA") sigue sin confirmación de elegibilidad Argentina específica — correctamente no puntuado, pendiente de verificación manual.

**Confirmación de priorización remote-friendly en Parte 2:** el modo remoto fue detectado y activado correctamente. La propuesta de distribución del próximo lote de 25 solicitudes de conexión prioriza 8 empresas remote-friendly confirmadas (Deel, GitLab, Nubank, VTEX, Kavak, Atlassian, Shopify, Stripe) — cumple el criterio de ≥50% a empresas remote-friendly para el modo remoto.

## Coaching de Debilidades de Entrevista

**Sección salteada.** `historial-entrevistas.md` tiene 0 entrevistas registradas — solo placeholders de template (`[tipo de pregunta]`, `[Fecha]`, etc.). No hay datos de patrones de debilidad sobre los cuales construir drills. Esto no bloquea el resto del briefing, pero vale notar: sin entrevistas reales en el pipeline, el coaching de debilidades seguirá vacío hasta que haya al menos una entrevista para debriefear con `/debrief-entrevista`.

## Stack de Prioridades de Hoy

1. **Enviar las 2 postulaciones de mayor score ya generadas y verificadas** — Deel Senior PM FinTech Payments/Credit Control & Risk (80/100, 49 días esperando) y Deel Staff PM Time & Workforce Management (79/100, 52 días esperando). Esta es la acción de mayor apalancamiento: no requiere generar nada nuevo, solo ejecutar lo que ya existe. Registrar el envío con `/rastrear-postulaciones agregar` inmediatamente después.
2. **Activar al menos 1 de los 6 pedidos de referido identificados en `rastreador-conexiones.md`** — empezar por Elena Yndurain (Microsoft, Director AI Product Management, el match más directo con la especialización en IA) o Pedro Alejandro Santamarina (Mercado Libre, el contacto de Product más senior en la red actual). Ejecutar `/pedir-referido [nombre] + [rol]`.
3. **Verificar manualmente los 2 leads pendientes de confirmación de recencia/elegibilidad** — GitLab "Product Manager, AI Editor Extensions" (confirmar si "Remote, Americas" incluye Argentina) y Deel "Country Product Manager — LATAM" en careers.deel.com directamente (47 días de antigüedad, pendiente de confirmación de recencia pero con elegibilidad Argentina explícita ya confirmada).
4. **Si hay tiempo:** exportar conexiones nuevas de LinkedIn y actualizar `rastreador-conexiones.md` (104 días sin tocar) — esto desbloquea el próximo lote real de 25 solicitudes de conexión que Parte 2 no pudo generar hoy por falta de datos.

Tiempo estimado: 30-35 minutos total (envío de 2 postulaciones + registro ~12 min, 1 pedido de referido ~8 min, verificación manual de 2 leads ~5 min, export de LinkedIn si hay tiempo ~10 min).
