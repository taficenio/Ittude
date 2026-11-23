# Parte 3: Pipeline y Coaching - Lunes, 23 de Noviembre de 2026

**Gate de calidad:** `plan-carrera.md` tiene datos reales (OK — detección de persona y coaching proceden). `historial-entrevistas.md` está vacío (solo placeholders de template, 0 entrevistas) — **se saltea la sección de Coaching de Debilidades de Entrevista**, no bloquea el resto. No existe `app-tracker.md` — el pipeline se reconstruye desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y los briefings de Partes 1-2 de hoy.

**Persona detectada (`plan-carrera.md`):** PM/PO Senior, abierto a IC/Lead-Head/especialización IA, remoto excluyente, sin empleo actual (gap real ~1 mes, no career gap), sin founder. → Aplica **Coaching de Candidato Remoto** únicamente.

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Ninguna postulación confirmada como enviada — ver nota abajo |
| Referido solicitado | 0 | 6 contactos prioritarios identificados, ninguno activado aún |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | — |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Nota crítica (no es un "0" vacío, es un "0" con trabajo acumulado sin enviar):** Día 106 del sistema (desde 2026-08-10), 0 postulaciones enviadas en total. Hay 3 CVs ya generados y verificados con score ≥70/100 esperando envío:
- Deel — Senior PM FinTech Payments/Credit Control & Risk — 80/100 — generado hace 47 días
- Deel — Staff PM Time & Workforce Management — 79/100 — generado hace 50 días
- VTEX — Order Management — 72/100 — generado hace 81 días

Y 6 pedidos de referido ya identificados (ver Parte 2 de hoy) sin un solo mensaje enviado en 102 días desde que se identificaron los contactos.

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen — pero no por falta de roles calificados, por falta de ejecución.**

El patrón estándar de "cero volumen" asume que falta encontrar roles 70+. Acá no es el caso: ya existen 3 CVs verificados por encima del umbral (80, 79 y 72), generados hace 47-81 días, y 6 referidos prioritarios identificados hace 102 días. El sistema generó el trabajo; nadie apretó "enviar". Esto no se arregla con más research ni más CVs — se arregla enviando lo que ya está listo.

Acción no negociable de hoy: enviar las 3 postulaciones generadas y activar al menos 2 de los 6 pedidos de referido. Ningún otro skill (`/evaluar-oferta`, `/adaptar-cv`, `/investigar-empresa`) debería correr hoy hasta que esto pase — generar un cuarto CV sin haber enviado los primeros tres sería repetir el mismo patrón que ya lleva 106 días.

---

## Coaching de Persona

### Candidato Remoto

Modalidad remoto excluyente confirmada en `plan-carrera.md` — filtro duro, no preferencia blanda. Cruce con Parte 1 de hoy: el escaneo de roles descartó correctamente por modalidad a Kavak ("AI Product Manager" en Buenos Aires, híbrido 3 días/semana) y a Nubank (Senior Staff PM Crypto, marcado híbrido) — ningún posting híbrido/presencial se coló como hallazgo válido. Parte 2 de hoy confirma que se activó MODO REMOTO y que la propuesta de distribución del próximo lote de 25 solicitudes de conexión prioriza 8 empresas remote-friendly (Deel, GitLab, Nubank, VTEX, Kavak, Atlassian, Shopify, Stripe) muy por encima del mínimo de 50% remote-friendly que exige el modo. El filtro de modalidad se está aplicando correctamente en ambas partes — sin corrección pendiente acá.

---

## Coaching de Debilidades de Entrevista

Salteado — `historial-entrevistas.md` no tiene entrevistas registradas (0 entrevistas, solo placeholders de template). No hay datos para medir patrones de debilidad. Esta sección se activará automáticamente una vez que se registre la primera entrevista real vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Enviar las 3 postulaciones ya generadas y verificadas** — Deel Senior PM FinTech (80/100), Deel Staff PM (79/100), VTEX Order Management (72/100). Son los únicos CVs del sistema que superan el umbral de 70 y llevan entre 47 y 81 días esperando. Esto es lo de mayor apalancamiento disponible hoy: cero trabajo nuevo necesario, solo ejecución.
2. **Activar 2 de los 6 pedidos de referido prioritarios** identificados en `rastreador-conexiones.md`: Elena Yndurain (Microsoft, Director AI Product Management — match directo con tu especialización en IA) y Pedro Alejandro Santamarina (Mercado Libre, Sr. Product Development Manager — contacto de Product más senior en tu red). Correr `/pedir-referido [nombre] + [rol]` para cada uno.
3. **Verificar manualmente los 2 leads de rol pendientes de confirmación** señalados en Parte 1: GitLab "Product Manager, AI Editor Extensions" (confirmar si "Remote, Americas" incluye Argentina) y Deel "Country Product Manager — LATAM" (confirmar recencia en careers.deel.com — el posting vía jobs.a16z.com ya tiene 45 días).
4. **Si hay tiempo:** actualizar `/rastrear-postulaciones` con el estado real de las 3 postulaciones enviadas hoy, y exportar conexiones nuevas de LinkedIn para refrescar `rastreador-conexiones.md` (102 días sin tocar — esto sigue limitando lo que Partes 1 y 2 pueden confirmar con certeza cada día).

Tiempo estimado: 45-60 minutos total
