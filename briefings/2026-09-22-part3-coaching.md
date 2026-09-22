# Parte 3: Pipeline y Coaching - Martes, 22 de septiembre de 2026

## Gate de Calidad

- `plan-carrera.md`: tiene datos reales -- briefing corre completo. Función objetivo detectada: **Product Manager / Product Owner** (Senior IC, Lead/Head, o especialización en IA -- los tres caminos siguen abiertos).
- `historial-entrevistas.md`: **vacío** (0 entrevistas registradas, solo placeholders de template) -- la sección de Coaching de Debilidades de Entrevista se saltea abajo, como indica el flujo cuando hay menos de 3 entrevistas.
- Pipeline: no existe `app-tracker.md` en el repo. Se arma el resumen de abajo desde `empresas-objetivo.md` (sin campos de Estado poblados, última actualización 2026-08-10), `rastreador-conexiones.md` (última actualización 2026-08-13) y los briefings de hoy (Parte 1 y Parte 2), que registran explícitamente **0 postulaciones enviadas, 0 entrevistas, 0 ofertas** desde el inicio del sistema.

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas desde el inicio del sistema |
| Referido solicitado | 0 | 6 mensajes de reconexión Tier C redactados (Parte 2, hoy y días anteriores) pero **sin confirmación de envío** -- no cuentan como "solicitado" hasta que haya fecha de contacto registrada |
| Entrevista programada | 0 | -- |
| Entrevistado (esperando resultado) | 0 | -- |
| Etapa de oferta | 0 | -- |
| Rechazado esta semana | 0 | -- |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana -- de hecho, sin postulaciones aún en 44 días desde que se generó `empresas-objetivo.md`. Enviar al menos 2 hoy.

Pero el diagnóstico real es más específico que "faltan candidatos": la Parte 1 de hoy identificó varios roles con fit temático fuerte (Bitso Product Manager Crypto Core, VTEX Product Manager Billing, Globant Product Manager Senior-Level con URL ya conocida, Stripe Product Manager LATAM) que no pasaron el gate automático de verificación solo porque `WebFetch` sigue bloqueado (`EGRESS_BLOCKED`, 44+ días) y no se pudo confirmar la fecha de publicación de forma automática. Eso no es lo mismo que "no hay roles 70+" -- es que el sistema no puede verificarlos solo. La acción correcta hoy no es expandir la lista de targets (ya tiene ~108 empresas), es **abrir manualmente 1-2 de esos links en el navegador**, confirmar fecha y elegibilidad a mano, y si el fit es real, correr `/puntuar-oferta` y postular.

Mismo patrón en networking (Parte 2): 40 días sin que se confirme el envío de ningún mensaje ya redactado. El cuello de botella de fondo, dos partes del sistema coincidiendo, no es research ni generación de contenido -- es la conversión de outputs ya generados en acciones reales (enviar, registrar, actualizar trackers).

---

## Coaching de Persona

### Candidato Remoto
`plan-carrera.md` marca modalidad remota como filtro duro ("Remoto excluyente", confirmado 2026-08-12). El sistema está aplicando el filtro correctamente: la Parte 1 de hoy descartó Kavak (híbrido confirmado, Ciudad de México) y volvió a confirmar Duolingo como híbrido, no remote-first. La Parte 2 cumplió el mínimo de 50% del lote de conexiones hacia empresas remote-friendly confirmadas (GitLab, Deel, Atlassian, Shopify, Remote.com).

**Pendiente sin resolver, 18 días:** Nubank sigue marcado como modalidad híbrida en `empresas-objetivo.md` sin una decisión registrada (pendiente desde 2026-09-04). Nubank es una de las 13 empresas Tier 1 y una fintech de alta afinidad con el perfil (conecta con el paso por Freeos/DeFi) -- vale la pena resolver hoy si el rol específico permite excepción al filtro duro o si se descarta definitivamente, en vez de dejarlo indefinido.

---

## Coaching de Debilidades de Entrevista

Salteado -- `historial-entrevistas.md` tiene 0 entrevistas registradas (mínimo del sistema: 3).

---

## Stack de Prioridades de Hoy

1. **Enviar al menos 1 postulación real.** Abrir manualmente en el navegador uno de los candidatos ya identificados hoy en la Parte 1 -- el más verificable es Globant "Product Manager Senior-Level" (`career.globant.com/job/product-manager/66302`, URL estable en búsquedas de varios días) o Stripe "Product Manager, LATAM" (fit de modalidad más limpio). Confirmar fecha y elegibilidad a mano, correr `/puntuar-oferta`, y si pasa el mínimo, `/adaptar-cv` y postular.
2. **Enviar los 6 mensajes de reconexión Tier C** ya redactados en la Parte 2 de hoy (Elena Yndurain, Virginia Silvero, Melina Ruggeri, María José Trejo Conde, Bernardo Manzella, Pedro Alejandro Santamarina) -- están listos desde hace días, solo falta apretar enviar.
3. **Resolver la decisión pendiente de Nubank** (híbrido, 18 días sin resolver) en `empresas-objetivo.md` -- descartar o marcar como excepción justificada.
4. **Si hay tiempo:** correr las 11 queries de LinkedIn de la Parte 2 y pegar los resultados para desbloquear el lote real de 25 solicitudes de conexión (40 días de bloqueo). Después de cualquier envío de hoy (postulación o mensaje), actualizar `rastreador-conexiones.md` y crear un `app-tracker.md` mínimo -- sin esto, el sistema seguirá reportando 0 en cada métrica aunque haya progreso real.

Tiempo estimado: 30-40 minutos total (día con más carga de lo habitual por el backlog acumulado de envíos pendientes).
