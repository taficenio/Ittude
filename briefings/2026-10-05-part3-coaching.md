# Parte 3: Pipeline y Coaching - Lunes, 5 de octubre de 2026

**Gate de calidad:** `plan-carrera.md` tiene datos reales (no placeholders) — continúa el output completo. `historial-entrevistas.md` está vacío (0 entrevistas registradas, solo placeholders de template) — se saltea la sección de Coaching de Debilidades de Entrevista, no bloquea el resto. No existe `app-tracker.md` — el resumen del pipeline se construye desde `empresas-objetivo.md`, `rastreador-conexiones.md`, `historial-entrevistas.md` y los briefings de hoy (Parte 1 y Parte 2), igual que en corridas anteriores.

**Detección de función objetivo (`plan-carrera.md`):** Product Manager / Product Owner (IC senior, Lead/Head, o especialización en IA). Modalidad remota excluyente confirmada — filtro duro. Mercado: Argentina, LatAm, USA, Canadá.

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas desde el inicio del sistema (día 56, 2026-08-10 → hoy). Confirmado en `briefings/2026-10-05-part1-roles.md` y `-part2-networking.md`. |
| Referido solicitado | 0 | `rastreador-conexiones.md` no tiene ningún campo de estado "solicitada → conectada" con fecha. Los 6 pedidos de referido de mayor prioridad (Elena Yndurain/Microsoft, Virginia Silvero/Globant, Melina Ruggeri/Salesforce, Maria Jose Trejo Conde/Mercado Libre, Bernardo Manzella/Globant, Pedro Alejandro Santamarina/Mercado Libre) están redactados en `briefings/2026-10-05-briefing.md` pero sin evidencia de envío (53+ días). |
| Entrevista programada | 0 | — |
| Entrevistado (esperando resultado) | 0 | — |
| Etapa de oferta | 0 | — |
| Rechazado esta semana | 0 | — |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Nota sobre el dato:** no es falta de output del sistema — hay 3 CVs generados y verificados listos para enviar (VTEX y Globant desde el 2026-09-03/2026-10-04, Deel generado hoy con Fit 79/100) y 25 solicitudes de conexión redactadas entre los tres archivos de hoy. El cuello de botella es 100% de envío, no de generación.

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana (ni en las 8 semanas anteriores). Enviar al menos 2 hoy — ya hay roles 70+ listos: VTEX (CV listo desde hace 32 días, el rol de Stripe análogo ya se perdió por esta misma demora) y Deel Staff PM (Fit 79/100, generado hoy, remoto confirmado desde Argentina). No hace falta expandir la lista de targets ni ajustar criterios en `plan-carrera.md` — el problema no es oferta, es acción.

---

## Coaching de Persona

### Candidato Remoto
`plan-carrera.md` confirma modalidad remota excluyente (filtro duro, actualizado 2026-08-12).

- **Escaneo de roles (Parte 1) revisado:** el escaneo de hoy ya aplicó el filtro correctamente — descartó explícitamente Mercado Libre, Stripe, GitLab, VTEX (roles no confirmados remotos), Notion, Duolingo, Anthropic (25%+ oficina) y Wise (híbrido, 2 días/semana) por no cumplir modalidad remota desde Argentina/LatAm. El único caso ambiguo activo es **Globant** (Product Manager Senior-Level) — modalidad no confirmada, empresa mayormente híbrida en Argentina. Correctamente marcado "no enviar hasta confirmar modalidad" en vez de descartarlo o enviarlo a ciegas.
- **Networking (Parte 2) priorizó remote-friendly:** confirmado — "MODO REMOTO activo", 4 de 8 solicitudes de conexión de hoy son empresas LatAm de operación regional remota (Buk, Betterfly, Lemon Cash, Addi); Anthropic y Hugging Face se mantuvieron por match de especialización en IA, con advertencia explícita de que su modalidad 100% remota no está confirmada.
- **Acción derivada:** el mensaje a Virginia Silvero (Globant, borrador ya listo en Parte 1) es el paso que resuelve la única ambigüedad de modalidad abierta hoy. Sin esa confirmación, el CV de Globant no debe enviarse — es un dealbreaker duro, no una preferencia blanda.

---

## Coaching de Debilidades de Entrevista

Salteado — `historial-entrevistas.md` tiene 0 entrevistas registradas (solo placeholders de template). No hay patrones de debilidad de los cuales partir. Esta sección se activará automáticamente después de la primera entrevista real vía `/debrief-entrevista`.

---

## Stack de Prioridades de Hoy

1. **Enviá las 2 postulaciones formales con CV ya generado y verificado:** VTEX (listo desde 2026-09-03, 32 días de demora — no repitas el patrón que le costó la vacante al CV de Stripe) y Deel Staff PM, Time & Workforce Management (Fit 79/100, generado hoy, cobertura ~90%, ATS PASA). Esto es lo único que mueve el pipeline de 0 a volumen real.
2. **Enviá el mensaje a Virginia Silvero** (Globant, borrador en `briefings/2026-10-05-part1-roles.md`) para confirmar modalidad remota antes de decidir sobre el CV de Globant — resuelve en minutos la única ambigüedad de modalidad abierta.
3. **Enviá las 8 solicitudes de conexión de Parte 2** (Anthropic ×2, Buk ×2, Hugging Face, Betterfly, Lemon Cash, Addi) más las 17 ya listas en `briefings/2026-10-05-briefing.md` — 25 en total hoy, directo contra el gap de cobertura de 99/108 empresas sin conexión de 1er grado.
4. Si hay tiempo: actualizá `rastreador-conexiones.md` con cada solicitud efectivamente enviada y corré `/rastrear-postulaciones agregar` para VTEX y Deel una vez postulado — sin esto, ninguna corrida futura puede detectar aceptaciones ni medir el pipeline real (el archivo no tiene una actualización real desde 2026-08-13).

Tiempo estimado: 35-40 minutos total (2 postulaciones formales + 1 mensaje de referido + 25 solicitudes de conexión + actualización de trackers).
