# Parte 3: Pipeline y Coaching - Martes, 17 de Noviembre de 2026

## Resumen del Pipeline

**Nota de fuente:** no existe `app-tracker.md` en el repo. Pipeline construido desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y los briefings de hoy (Parte 1 y Parte 2). Ningún número de esta tabla fue inventado — donde no hay evidencia de un estado, se registra 0.

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones enviadas registradas — ver nota abajo sobre los 3 CVs listos |
| Referido solicitado | 0 | `rastreador-conexiones.md` no tiene ningún campo de "Referido solicitado" poblado con fecha de envío |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | `historial-entrevistas.md` registra 0 entrevistas (solo placeholders de template) |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Lo que sí existe, listo para enviar y sin estado de "postulado" porque nunca se envió:**
- Deel — Senior PM, FinTech Payments/Credit Control & Risk — score 80/100 — CV generado, **41 días esperando el envío**
- Deel — Staff PM, Time & Workforce Management — score 79/100 — CV generado, **44 días esperando el envío**
- VTEX — Order Management — score 72/100 — CV generado, **~75 días esperando el envío**
- Globant — Product Manager Senior-Level — bloqueado por confirmación de modalidad pendiente (no cuenta como listo)

Estos 3 CVs verificados (80, 79, 72/100) son trabajo ya hecho por el sistema que no se tradujo en ninguna postulación real en más de 40 días en los dos casos más viejos.

---

## Verificación de Salud del Pipeline

**Cero volumen** (0 postulaciones esta semana, y de hecho 0 en los 100 días desde que el sistema empezó a correr el 2026-08-10):

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana — ni en ninguna semana anterior. Enviar al menos 2 hoy. No hace falta generar más roles ni expandir la lista de targets: ya hay 3 CVs con score ≥70/100 generados y verificados (Deel 80/100, Deel 79/100, VTEX 72/100) que llevan entre 41 y 75 días sin enviarse. El trabajo de research y adaptación ya está hecho — el paso que falta es apretar "enviar".

Esto no es un problema de que el sistema no esté generando suficiente output: es un problema de que el output generado no se está convirtiendo en acción. Generar un quinto CV o escanear una empresa número 19 no mueve el pipeline. Enviar los 3 que ya existen, sí.

---

## Coaching de Persona

### Candidato Remoto

`plan-carrera.md` confirma modalidad **Remoto excluyente** (filtro duro, actualizado 2026-08-12) — se activa el modo correspondiente.

- **Escaneo de híbrido/presencial (Parte 1 de hoy):** confirmado funcionando como guardarraíl — de las 18 empresas revisadas, varios roles PM reales fueron descartados explícitamente por modalidad no remota (Microsoft, Amazon, Apple, Google, Salesforce presencial/sin tag remoto en BA, Kavak híbrido 3 días/semana, Nubank con ciclos de oficina cada 8-12 semanas, Duolingo híbrido/restringido a oficinas en US). El filtro duro está haciendo su trabajo — no se está colando ningún rol que violaría la preferencia.
- **Priorización remote-friendly en Parte 2 de hoy:** confirmada — 7 de las 8 empresas del próximo lote de 25 solicitudes de conexión (Deel, GitLab, Nubank, VTEX, Kavak, Atlassian, Shopify) son remote-friendly confirmadas, cumpliendo el mínimo de 50% del modo remoto.

No hay advertencia nueva que agregar sobre modalidad hoy — el sistema está respetando el filtro correctamente en ambas partes.

---

## Coaching de Debilidades de Entrevista

**Sección salteada.** `historial-entrevistas.md` registra 0 entrevistas (solo placeholders de template: "Total de entrevistas: 0", sin ningún log real). No hay datos de debilidades que coachear todavía — esto se activa automáticamente después de la primera entrevista real vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Enviar los 3 CVs ya verificados y listos** — Deel Senior PM FinTech (80/100), Deel Staff PM Time & Workforce (79/100), VTEX Order Management (72/100). Cero trabajo nuevo de research o redacción: son postulaciones que ya pasaron por `/adaptar-cv` + revisión de reclutador/ATS y llevan entre 41 y 75 días esperando. Después de cada envío, correr `/rastrear-postulaciones agregar` para que el pipeline deje de mostrar 0.
2. **Verificar manualmente el lead de Deel "Country Product Manager — LATAM"** en careers.deel.com (remoto, USD 65-105K, cobertura explícita Argentina) — es el único hallazgo con elegibilidad Argentina explícita entre las 18 empresas revisadas hoy en Parte 1, solo le falta confirmación de recencia.
3. **Activar 1-2 de los 6 pedidos de referido ya identificados** en `rastreador-conexiones.md` (Elena Yndurain – Microsoft, Virginia Silvero o Bernardo Manzella – Globant, Melina Ruggeri – Salesforce, Maria Jose Trejo Conde o Pedro Alejandro Santamarina – Mercado Libre). Correr `/pedir-referido [nombre] + [rol]` para generar el mensaje — llevan 96 días identificados sin enviarse.
4. **Si hay tiempo:** exportar conexiones nuevas de LinkedIn y actualizar `rastreador-conexiones.md` (última actualización real: 2026-08-13, 96 días sin tocar) — esto desbloquea que la próxima corrida de Parte 2 pueda generar el lote real de 25 solicitudes de conexión en vez de quedar bloqueada por falta de datos frescos.

Tiempo estimado: 25-30 minutos total (los pasos 1 y 3 son principalmente enviar/pegar contenido ya generado, no crear nada nuevo).
