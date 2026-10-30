# Parte 3: Pipeline y Coaching - Viernes, 30 de octubre de 2026

**Contexto de la corrida:** `git pull origin main` traído al inicio — repo al día. Función objetivo detectada en `plan-carrera.md`: Product Manager / Product Owner (IC senior, Lead/Head, o especialización en IA — tres caminos abiertos). No existe `app-tracker.md` en el repo — el pipeline de abajo se reconstruye desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y `briefings/2026-10-30-briefing.md` (que ya trae un resumen de pipeline consolidado de hoy).

**Gate de calidad:** `plan-carrera.md` tiene datos reales (no placeholders) → se continúa con coaching de persona completo. `historial-entrevistas.md` tiene 0 entrevistas registradas (solo placeholders de template) → se salta la sección de coaching de debilidades de entrevista, sin bloquear el resto del output.

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | 4 CVs generados y verificados (score ≥70/100) esperando envío humano: Deel Senior PM FinTech (80/100, 23 días esperando desde 2026-10-07), Deel Staff PM Time & Workforce Management (79/100, 26 días esperando desde 2026-10-04), VTEX Order Management (57 días esperando desde 2026-09-03), Globant PM Senior-Level (bloqueado por confirmación de modalidad pendiente) |
| Referido solicitado | 0 | 6 conexiones de 1er grado de alta prioridad identificadas desde el 2026-08-13, ninguna marcada como contactada en `rastreador-conexiones.md` |
| Entrevista programada | 0 | Ninguna |
| Entrevistado (esperando resultado) | 0 | Ninguna |
| Etapa de oferta | 0 | Ninguna |
| Rechazado esta semana | 0 | Ninguno |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Nota de confiabilidad del dato:** `rastreador-conexiones.md` no se actualiza desde 2026-08-13 (78 días), y no existe ningún registro de postulación formal en el sistema (vía `/rastrear-postulaciones`) en los 82 días desde el día 1. Estas cifras seguirán en cero en cada corrida futura mientras no se registren envíos reales — no es evidencia de que no haya material listo para enviar (ver 4 CVs arriba).

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones enviadas en 82 días desde el día 1 del sistema (12 semanas y 5 días), y sin ninguna esta semana. A diferencia del escenario de "cero volumen" por falta de roles válidos, acá **sí hay roles ≥70/100 ya generados y verificados** — dos de Deel (79 y 80/100) llevan 23-26 días listos, y uno de VTEX lleva 57 días. No hace falta expandir la lista de targets ni ajustar criterios en `plan-carrera.md`: el gate de calidad ya está pasado. El cuello de botella es puramente de envío humano, no de generación ni de criterio.

**Acción concreta:** Enviar al menos 2 de las 4 postulaciones ya generadas hoy (Deel Senior PM FinTech y Deel Staff PM son las de score más alto). Después de cada envío, correr `/rastrear-postulaciones agregar` para que el pipeline real quede registrado y las corridas futuras puedan medir conversión en vez de seguir reportando ceros.

---

## Coaching de Persona

### Candidato Remoto

`plan-carrera.md` confirma modalidad remota excluyente como filtro duro ("ni roles híbridos ni presenciales, aunque el resto del fit sea fuerte"). Chequeo cruzado:

- **Escaneo de roles de hoy** (`briefings/2026-10-30-briefing.md`, sección "Roles Top Hoy"): no se verificó ningún rol nuevo hoy (13 búsquedas Tier 1, 0 roles que pasaran el gate de verificación de 24h + elegibilidad LatAm explícita), por lo que no hay ninguna advertencia de híbrido/presencial que reportar — no porque el filtro no se haya aplicado, sino porque no entró ningún candidato a evaluar.
- **Parte 2 (networking) de hoy:** confirma explícitamente "MODO REMOTO activo" y priorizó Betterfly (remoto, Chile) como única empresa con leads verificados — consistente con el filtro duro.

No hay acción adicional de este bloque hoy más allá de mantener el filtro al evaluar cualquier rol nuevo que aparezca.

*(Las secciones de Career Returner, Director+/Empleado y Founder a Empleado no aplican: el gap de empleo actual es de ~1-2 meses y ya está resuelto como transición normal en `plan-carrera.md`, no hay empleo actual que condicione el bloque matutino, y no hay antecedente de founder/CEO en la biblioteca de experiencias.)*

---

## Coaching de Debilidades de Entrevista

Se salta esta sección. `historial-entrevistas.md` tiene 0 entrevistas registradas (solo placeholders de template) — no hay datos suficientes (mínimo 3 entrevistas) para identificar patrones de debilidad ni generar drills específicos. En cuanto se registre la primera entrevista real vía `/debrief-entrevista`, esta sección empieza a poblarse.

---

## Stack de Prioridades de Hoy

1. **Enviar al menos 2 de las 4 postulaciones ya generadas y verificadas:** Deel Senior PM FinTech (80/100, 23 días esperando) y Deel Staff PM Time & Workforce Management (79/100, 26 días esperando) — es la acción que rompe directamente el cuello de botella de volumen.
2. **Enviar las solicitudes de conexión frescas antes de que pierdan vigencia:** Katherin Bracho (Betterfly, lead de hoy vía Parte 2) y los 2 leads de ayer aún sin enviar (Uriel Kejsefman – Duolingo, Flor Reyes – Anthropic).
3. **Enviar el mensaje a Virginia Silvero (Globant)** para confirmar modalidad y desbloquear el cuarto CV ya generado, bloqueado hace semanas.
4. **Si hay tiempo:** correr `/rastrear-postulaciones agregar` después de cada envío real de hoy, y exportar un CSV fresco de LinkedIn para refrescar `rastreador-conexiones.md` (78 días sin actualizar).

Tiempo estimado: 20 minutos total
