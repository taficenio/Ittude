# Parte 3: Pipeline y Coaching - Viernes, 27 de Noviembre de 2026

## Gate de Calidad

- **plan-carrera.md:** datos reales, no placeholders. OK para continuar con detección de persona y coaching.
- **historial-entrevistas.md:** vacío (0 entrevistas registradas, solo placeholders de template). La sección de Coaching de Debilidades de Entrevista se saltea más abajo — no hay datos para analizar.
- **Pipeline:** no existe `app-tracker.md` en el repo. Resumen armado desde fuentes alternativas: `empresas-objetivo.md` (generado 2026-08-10, sin campos de Estado poblados por postulación), `rastreador-conexiones.md` (última actualización real: 2026-08-13 — 106 días sin tocar), `historial-entrevistas.md` (0 registros) y los briefings de Parte 1 y Parte 2 de hoy (`briefings/2026-11-27-part1-roles.md`, `briefings/2026-11-27-part2-networking.md`).

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Ninguna postulación enviada registrada en 110 días de sistema (día 1: 2026-08-10) |
| Referido solicitado | 0 | 6 contactos prioritarios identificados, ninguno activado (106 días desde identificación) |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | — |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Dato clave que no entra en la tabla de etapas:** hay 3 CVs ya generados y verificados con score ≥70/100, listos para enviar y sin evidencia de envío:
- Deel — Senior PM FinTech (Payments/Credit Control & Risk) — 80/100 — generado hace 51 días
- Deel — Staff PM Time & Workforce Management — 79/100 — generado hace 54 días
- VTEX — Order Management — 72/100 — generado hace 85 días

Esto no es un problema de research o de scoring — el trabajo de generación y verificación ya está hecho. Es un problema de ejecución: nada de lo ya construido se está enviando.

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones enviadas esta semana — ni en ninguna semana de los 110 días del sistema. A diferencia del caso genérico de "cero volumen", acá el problema no es falta de roles con score 70+: ya existen 3 (Deel 80/100, Deel 79/100, VTEX 72/100), generados y verificados hace entre 51 y 85 días. Expandir la lista de targets o ajustar criteria en `plan-carrera.md` no es la palanca correcta hoy. La acción es enviar lo que ya está listo — hoy, no otro CV nuevo.

Los otros checks de salud (alto volumen sin referidos, referidos sin convertir, entrevistas sin prep) no aplican: no hay volumen de postulaciones ni de referidos sobre el cual medirlos todavía.

---

## Coaching de Persona

### Candidato Remoto (activado — `plan-carrera.md` indica modalidad "Remoto excluyente", filtro duro)

- Parte 1 de hoy escaneó 18 empresas y descartó explícitamente varios roles por modalidad híbrida o presencial (ej. Mercado Pago "UX Project Leader" en Buenos Aires, Kavak "AI Product Manager" híbrido 3 días/semana) — el filtro remoto se está aplicando de forma consistente, no hay fuga de roles no-remotos coladas en el pipeline.
- Parte 2 de hoy priorizó explícitamente 8 empresas remote-friendly confirmadas (Deel, GitLab, Nubank, VTEX, Kavak, Atlassian, Shopify, Stripe) para el próximo lote de solicitudes de conexión, en línea con el modo remoto activado.
- No hay otras personas de plan-carrera.md activas: el usuario no es career returner (el gap real es ~1 mes de transición, no un gap de carrera que amerite programas de returnship), no es Director+/empleado actualmente (no está empleado) y no es founder-a-empleado.

---

## Coaching de Debilidades de Entrevista

Salteado — `historial-entrevistas.md` tiene 0 entrevistas registradas (solo placeholders de template). No hay datos de patrones de debilidad ni entrevistas programadas con las cuales cruzar. Esta sección se reactivará automáticamente después de la primera entrevista real registrada vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Enviar las 3 postulaciones ya generadas y verificadas** — Deel Senior PM FinTech (80/100), Deel Staff PM Time & Workforce Management (79/100), VTEX Order Management (72/100). No requieren más research ni generación — es acción directa de envío. Después de enviar cada una, correr `/rastrear-postulaciones agregar` para que quede en el tracker.
2. **Verificar manualmente y aplicar al lead de Deel reconfirmado hoy** — "Country Product Manager — LATAM" (`jobs.a16z.com/jobs/deel/a052003d-4a6c-4f96-b1d0-cbb41635b116--country-product-manager-latam`), remoto, requiere base en LatAm, USD 65-105K, 49 días de antigüedad.
3. **Activar al menos 1 de los 6 pedidos de referido ya identificados** — Elena Yndurain (Microsoft), Virginia Silvero o Bernardo Manzella (Globant), Melina Ruggeri (Salesforce), Maria Jose Trejo Conde o Pedro Alejandro Santamarina (Mercado Libre). Correr `/pedir-referido [nombre] + [rol]`.
4. **Si hay tiempo:** exportar conexiones nuevas de LinkedIn y actualizar `rastreador-conexiones.md` (106 días sin tocar) — desbloquea el próximo lote real de 25 solicitudes de conexión en la próxima Parte 2.

Tiempo estimado: 30-40 minutos total
