# Parte 3: Pipeline y Coaching - Viernes, 9 de Octubre de 2026

## Resumen del Pipeline

**Fuente:** No existe `app-tracker.md` en el repo. Pipeline reconstruido desde `empresas-objetivo.md`, `rastreador-conexiones.md` e `historial-entrevistas.md`, cruzado con los outputs de hoy (`2026-10-09-part1-roles.md`, `2026-10-09-part2-networking.md`). Mismo patrón que viene señalando el sistema desde hace semanas: cero actividad registrada de postulación o referido formal, pese a que sí hay trabajo generado esperando envío.

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas. 4 CVs generados y verificados esperando envío humano: Deel Senior PM FinTech (score 80/100, generado 2026-10-07), Deel Staff PM Time & Workforce Management (score 79/100, generado 2026-10-04), VTEX Order Management (36 días de demora desde 2026-09-03), Globant PM Senior-Level (bloqueado por confirmación de modalidad pendiente) |
| Referido solicitado | 0 | Ninguno marcado como enviado en `rastreador-conexiones.md`. 6 conexiones de 1er grado de alta prioridad identificadas y sin usar (Elena Yndurain - Microsoft, Virginia Silvero - Globant, Melina Ruggeri - Salesforce, Maria Jose Trejo Conde - Mercado Libre, Bernardo Manzella - Globant, Pedro Alejandro Santamarina - Mercado Libre) |
| Entrevista programada | 0 | Ninguna |
| Entrevistado (esperando resultado) | 0 | Ninguna |
| Etapa de oferta | 0 | Ninguna |
| Rechazado esta semana | 0 | Ninguno |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

**Nota:** `rastreador-conexiones.md` no se actualiza desde 2026-08-13 (57 días). Mientras no se registren envíos reales (postulaciones, solicitudes de conexión, pedidos de referido), estas métricas seguirán en cero en cada corrida futura — no porque no haya actividad planeada, sino porque no se está registrando.

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana (0 postulaciones en 9 semanas de búsqueda). A diferencia del criterio por defecto de este chequeo, el problema acá no es falta de roles 70+: el sistema ya generó y verificó **4 CVs con score igual o mayor a 70/100**, dos de ellos (Deel, 79 y 80/100) listos desde hace 2-5 días. La variable que no se está moviendo es 100% acción humana — enviar lo que ya está hecho.

**Acción concreta:** Enviar al menos 2 de las 4 postulaciones ya generadas hoy. No hace falta expandir la lista de targets ni ajustar `plan-carrera.md` — el gate de calidad ya está pasado para estos 4 roles. Después de enviar, correr `/rastrear-postulaciones agregar` para cada una, así el pipeline real queda registrado y las corridas futuras pueden medir conversión.

---

## Coaching de Persona

### Candidato Remoto

`plan-carrera.md` confirma modalidad remota excluyente como filtro duro (actualizado 2026-08-12): ningún rol híbrido o presencial se considera, sin importar el resto del fit.

- **Escaneo de roles de hoy (Parte 1):** sin advertencias de híbrido/presencial coladas — los roles marcados "no se pudo verificar" (VTEX, Stripe, Anthropic) quedaron así precisamente porque `WebFetch` no pudo confirmar en la fuente primaria la elegibilidad remota desde LatAm, no porque hayan pasado el filtro con un dato dudoso. Globant sigue bloqueado por la misma razón: falta confirmar modalidad con Virginia Silvero antes de enviar ese CV.
- **Priorización de empresas remote-friendly (Parte 2):** el lote de solicitudes de conexión de hoy (7 en total: Rappi, Ualá, NotCo, Stone Co x2, iFood x2) **no cumplió el umbral de 50% remote-friendly** que exige MODO REMOTO — las 10 empresas explícitamente remote-friendly intentadas (Vercel, PagerDuty, ServiceNow, Linear, Rippling, Siigo, Automattic, Zapier, PostHog, Grammarly) no rindieron ningún prospecto verificable hoy. El propio briefing de Parte 2 señala el gap con honestidad en vez de forzar el cumplimiento. **Acción recomendada:** si el acceso de red mejora en próximas corridas, repriorizar esas 10 empresas remote-friendly antes de seguir sumando LatAm genérico, para no sesgar el pipeline hacia empresas sin política remota explícita.

---

## Coaching de Debilidades de Entrevista

Saltear esta sección. `historial-entrevistas.md` tiene 0 entrevistas registradas (solo placeholders de template) — no hay datos suficientes (mínimo 3 entrevistas) para identificar patrones de debilidad ni generar drills específicos. En cuanto se registre la primera entrevista real vía `/debrief-entrevista`, esta sección empieza a poblarse.

---

## Stack de Prioridades de Hoy

1. **Enviar al menos 2 de las 4 postulaciones ya generadas y verificadas:** Deel Senior PM FinTech (80/100) y Deel Staff PM Time & Workforce Management (79/100) son las más fuertes y las más demoradas en espera de envío. Esto resuelve directamente el cuello de botella de volumen — el trabajo de generación ya está hecho.
2. **Enviar el mensaje a Virginia Silvero (Globant)** para confirmar modalidad y desbloquear el cuarto CV generado (36+ días bloqueado).
3. **Correr `/pedir-referido` para Elena Yndurain (Microsoft)** — Director AI Product Management, el match de red más directo con la especialización en IA, y la conexión prioritaria que lleva más tiempo sin usarse.
4. **Si hay tiempo:** actualizar `rastreador-conexiones.md` con cualquier solicitud de conexión, pedido de referido o postulación efectivamente enviada hoy (incluidas las 7 solicitudes de conexión de la Parte 2) — sin este registro, el pipeline seguirá midiendo 0/0/0 indefinidamente aunque haya actividad real.

Tiempo estimado: 25 minutos total
