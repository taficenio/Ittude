# Parte 3: Pipeline y Coaching - Miércoles, 16 de septiembre de 2026

## Resumen del Pipeline

**Fuente:** no existe `app-tracker.md` en el repo. Armado desde `empresas-objetivo.md` (108 empresas, sin campos de Estado poblados desde su generación el 2026-08-10), `rastreador-conexiones.md` (última actualización 2026-08-13), `historial-entrevistas.md` (vacío, 0 entrevistas) y los briefings de Parte 1 y Parte 2 de hoy.

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | 0 | Sin postulaciones registradas desde el inicio del sistema (38 días) |
| Referido solicitado | 0 | 6 contactos prioritarios identificados en `rastreador-conexiones.md`, ninguno con pedido activado todavía |
| Entrevista programada | 0 | |
| Entrevistado (esperando resultado) | 0 | |
| Etapa de oferta | 0 | |
| Rechazado esta semana | 0 | |

**Total de postulaciones activas:** 0
**Entrevistas esta semana:** 0

---

## Verificación de Salud del Pipeline

**TU CUELLO DE BOTELLA: Volumen.** Sin postulaciones aún esta semana — de hecho, sin postulaciones desde el día 1 del sistema (38 días). Enviar al menos 2 hoy. Si no hay roles 70+, expandir la lista de targets o ajustar criteria en `plan-carrera.md`.

Con el agravante de que esta vez el volumen cero no es por falta de esfuerzo — es un bloqueo estructural: `WebFetch` lleva **40 días consecutivos** devolviendo `EGRESS_BLOCKED` (verificado hoy en Parte 1 contra `stripe.com`, `job-boards.greenhouse.io` y `linkedin.com`), lo que le impide al sistema confirmar fecha de publicación y elegibilidad remota LatAm de cualquier hallazgo de `WebSearch` — el mínimo exigido por el gate de calidad de datos antes de puntuar un rol. Resultado: ningún rol puede puntuarse, y por lo tanto ninguna postulación puede generarse automáticamente. El único hallazgo cercano de hoy (GitLab — "Senior Platform Product Manager, Cloud Connector", remoto worldwide, deadline 9 de octubre) quedó sin puntuar por falta de fecha de publicación confirmable y de confirmación explícita de elegibilidad LatAm.

**Esto no lo resuelve el OS solo.** Mientras `WebFetch` siga bloqueado, la vía de mayor apalancamiento real es la manual: verificar el rol de GitLab por navegador y accionar los 6 pedidos de referido ya identificados (ver Coaching de Persona abajo), que no dependen de `WebFetch` en absoluto.

---

## Coaching de Persona

### Candidato Remoto
`plan-carrera.md` marca **remoto excluyente** como filtro duro (actualizado 2026-08-12): ningún rol híbrido o presencial se acepta, sin importar el resto del fit.

- Parte 1 de hoy no registró ningún hallazgo nuevo con alerta de híbrido/presencial que haya pasado el filtro — Anthropic, Nubank, Deel, GitLab y HubSpot se revisaron sin producir un rol puntuable, así que no hubo riesgo de colar un híbrido esta ronda.
- Parte 2 confirmó que las 18 solicitudes de conexión generadas hoy apuntan a empresas 100% remote-friendly (GitLab, Deel, Nubank, VTEX, HubSpot, Twilio, Zendesk, GitHub, PayPal, Shopify), cumpliendo el mínimo de MODO REMOTO. Además, Parte 2 deprioritizó explícitamente Amazon, Apple y Google esta ronda por ser roles mayormente presenciales/híbridos en HQ — coherente con el filtro duro.

---

## Coaching de Debilidades de Entrevista

`historial-entrevistas.md` tiene 0 entrevistas registradas (menos de 3) — sección salteada según la regla del sistema. No hay datos de debilidades de entrevista todavía para generar coaching.

---

## Stack de Prioridades de Hoy

1. **Activar un pedido de referido.** De los 6 contactos prioritarios en `rastreador-conexiones.md` con relevancia directa (Elena Yndurain — Microsoft, Director AI PM; Virginia Silvero — Globant, Regional Recruiter Lead; Melina Ruggeri — Salesforce, LATAM Recruiting Sr Manager; Maria Jose Trejo Conde — Mercado Libre, Talent Acquisition IT regional; Bernardo Manzella — Globant, Head of People & Capacity Strategy/AI Studios; Pedro Alejandro Santamarina — Mercado Libre, Sr. Product Development Manager), ejecutar `/pedir-referido` para al menos uno. Esta recomendación lleva **7 semanas seguidas** apareciendo sin acción — es la palanca de mayor conversión disponible en todo el sistema hoy.
2. **Verificar manualmente el hallazgo de GitLab** ("Senior Platform Product Manager, Cloud Connector", remoto worldwide, deadline 9 oct) vía navegador — confirmar fecha de publicación y elegibilidad LatAm explícita. Si pasa el gate, correr `/puntuar-oferta` y, si el score es 70+, `/adaptar-cv`.
3. **Enviar un primer lote de las 18 solicitudes de conexión** generadas en `2026-09-16-part2-networking.md` (empezar por las de mayor prioridad de cobertura: GitLab y Nubank). Marcar como enviadas en `rastreador-conexiones.md` al hacerlo — hoy ninguna de las solicitudes de briefings anteriores está marcada como enviada, lo que rompe el seguimiento de "Recién Conectados" en Parte 2.
4. **Si hay tiempo:** sumarte al Slack de Product School o a la comunidad de Lenny y comentar en 2-3 threads sobre AI product management (sugerencia de networking virtual de Parte 2).

Tiempo estimado: 30-35 minutos
