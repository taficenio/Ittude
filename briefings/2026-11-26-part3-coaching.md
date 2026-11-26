# Parte 3: Pipeline y Coaching - Jueves, 26 de Noviembre de 2026

**Gate de calidad:** `plan-carrera.md` tiene datos reales — OK para continuar. `historial-entrevistas.md` solo tiene placeholders de template (0 entrevistas registradas) — se saltea la sección de Coaching de Debilidades de Entrevista más abajo, como indica el flujo. No existe `app-tracker.md` — el resumen del pipeline se armó desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y los briefings de hoy (Parte 1 y Parte 2).

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin evidencia de envío. 3 CVs ya generados y verificados (score ≥70/100) siguen esperando: Deel Senior PM FinTech Payments/Credit Control & Risk (80/100, 50 días), Deel Staff PM Time & Workforce Management (79/100, 53 días), VTEX Order Management (72/100, 84 días) |
| Referido solicitado | 0 | 6 contactos prioritarios identificados en `rastreador-conexiones.md`, ninguno activado en 105 días |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | — |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Contexto:** Día 109 desde el inicio del sistema (2026-08-10), Semana 16. Cero postulaciones enviadas hasta la fecha. `rastreador-conexiones.md` no se actualizó con datos reales desde 2026-08-13 (105 días).

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana — ni en ninguna semana desde que arrancó el sistema. A diferencia del criterio estándar de este check ("si no hay roles 70+, expandir la lista de targets"), acá **sí hay roles 70+ ya generados y verificados**: Deel Senior PM FinTech (80/100), Deel Staff PM (79/100) y VTEX Order Management (72/100). El problema no es falta de roles calificados ni falta de proceso — es que lo que el sistema ya produjo y validó no se está enviando. Enviar las 3 postulaciones ya listas hoy es la acción de mayor apalancamiento disponible, sin trabajo adicional de generación.

En paralelo, los 6 contactos de referido prioritarios (Elena Yndurain, Virginia Silvero, Bernardo Manzella, Melina Ruggeri, Maria Jose Trejo Conde, Pedro Alejandro Santamarina) llevan 105 días identificados sin un solo mensaje enviado — esto va a limitar la tasa de respuesta de las 3 postulaciones en frío de arriba. Referido y postulación no son secuenciales; pueden salir hoy mismo en paralelo.

---

## Coaching de Persona

**Modo detectado (`plan-carrera.md`):** Candidato Remoto — "Remoto excluyente" es un filtro duro (actualizado 2026-08-12), sin roles híbridos ni presenciales.

Revisando el escaneo de roles de la Parte 1 de hoy: dos leads marcados con advertencia de modalidad (GitLab "AI Editor Extensions" — ubicación sin confirmar elegibilidad Argentina en el snippet, y Kavak AI PM — marcado híbrido 3 días en casa/resto oficina por la fuente consultada) quedaron correctamente sin puntuar por falta de confirmación de remoto, en línea con el filtro duro del plan de carrera. La Parte 2 de hoy confirma que priorizó el próximo lote de solicitudes de conexión hacia 8 empresas remote-friendly (Deel, GitLab, Nubank, VTEX, Kavak, Atlassian, Shopify, Stripe) — consistente con Modo Remoto.

No aplican los demás modos de persona: Career Returner (el gap real es de ~1 mes, no un gap de carrera — ver Debilidad 2 de `plan-carrera.md`), Director+/Empleado (el usuario no está empleado actualmente y el nivel objetivo no es exclusivamente Director+) y Founder a Empleado (sin roles de founder/CEO en la experiencia documentada).

---

## Coaching de Debilidades de Entrevista

Sección salteada — `historial-entrevistas.md` solo contiene placeholders de template (0 entrevistas registradas). Sin datos de entrevistas reales todavía no hay patrones de debilidad que calificar ni drills que recomendar. Esto se habilita automáticamente después de la primera entrevista real registrada vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Enviar las 3 postulaciones ya generadas y verificadas** — Deel Senior PM FinTech Payments/Credit Control & Risk (80/100, 50 días esperando), Deel Staff PM Time & Workforce Management (79/100, 53 días esperando), VTEX Order Management (72/100, 84 días esperando). No requieren más trabajo de generación, solo envío. Después de enviar cada una, correr `/rastrear-postulaciones agregar` para que el pipeline deje de depender de fuentes alternativas.
2. **Activar 1-2 de los 6 pedidos de referido prioritarios** — empezar por Elena Yndurain (Microsoft, Director AI Product Management — match directo con la especialización en IA) o Pedro Alejandro Santamarina (Mercado Libre, Sr. Product Development Manager — el contacto de Product más senior en la red actual). Correr `/pedir-referido [nombre] + [rol]`.
3. **Verificar manualmente los 2 leads pendientes de la Parte 1 de hoy** — GitLab "Product Manager, AI Editor Extensions" (confirmar elegibilidad Argentina directamente en el board) y Deel "Country Product Manager — LATAM" en careers.deel.com (bloqueado por red en esta sesión).
4. **Si hay tiempo:** exportar conexiones nuevas de LinkedIn y actualizar `rastreador-conexiones.md` (105 días sin tocar) — esto desbloquea el próximo lote real de 25 solicitudes de conexión que la Parte 2 de hoy no pudo generar por falta de datos frescos.

Tiempo estimado: 35 minutos total
