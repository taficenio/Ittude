# Parte 2: Networking - Martes, 17 de Noviembre de 2026

**Gate de calidad:** `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) — OK para continuar. `rastreador-conexiones.md` tiene datos reales pero **su última actualización registrada es 2026-08-13 — 96 días sin tocar**, igual que señaló Parte 1 hoy. Esto limita lo que esta corrida puede confirmar con certeza (ver nota en Seguimientos).

**Modo detectado (`plan-carrera.md`):** Función = Product Management (PM/PO, abierto a IC Senior / Lead-Head / especialización IA). Modalidad = **Remoto excluyente** (filtro duro) → se activa **MODO REMOTO**. No aplica Modo Director+/Empleado (el usuario no está empleado actualmente — ver Debilidad 2 del plan de carrera — y el nivel objetivo no es Director+). No aplica Modo Returner (el gap real es de ~1 mes, no un career gap que amerite reactivación de red dormida).

---

## ⚠️ Nuevas Solicitudes de Conexión — bloqueadas por falta de datos de LinkedIn, no se fabricaron 25 personas

Siguiendo `/solicitud-conexion`: Claude no puede buscar en LinkedIn directamente, y la regla central del OS es **nunca generar un mensaje para una persona o conexión que no sea real**. No hay perfiles de LinkedIn cargados en esta sesión desatendida para las empresas con gap, así que no se generaron 25 filas de tabla con nombres — eso habría significado inventar personas, lo cual el propio skill prohíbe explícitamente ("Do not generate a generic message" / "flag the person as needs manual research").

En vez de eso, esto es lo que sí se puede hacer con los datos reales disponibles:

### Empresas con gap de cobertura (menos de 4 conexiones en `rastreador-conexiones.md`)

Prácticamente todas las empresas objetivo tienen gap — 99 de 108 no tienen ninguna conexión, y Amazon (3), Apple (2), Google (2), Salesforce (2) y Atlassian (1) están por debajo del umbral. Solo Globant (16), Mercado Libre (16) y Microsoft (5) están cubiertas.

### Distribución propuesta del próximo lote de 25 (round-robin, ≥50% a empresas remote-friendly confirmadas por MODO REMOTO)

| Empresa | Conexiones actuales | Cupo propuesto | Remote-friendly confirmado |
|---|---|---|---|
| Deel | 0 | 4 (prioridad — lead de rol activo en Parte 1) | Sí — "Global/remoto", infraestructura EOR |
| GitLab | 0 | 3 | Sí — 100% remota desde su fundación |
| Nubank | 0 | 3 | Sí — remoto dentro de la región |
| VTEX | 0 | 3 | Sí — remoto regional |
| Kavak | 0 | 3 | Sí — remoto regional |
| Atlassian | 1 | 3 | Sí — cultura remote-first |
| Shopify | 0 | 3 | Sí — remote-first declarado |
| Stripe | 0 | 3 | No marcado explícito, pero Tier 1 / INTEL AVAILABLE |

Total: 25. 7 de 8 empresas (87.5% del lote) son remote-friendly confirmadas — cumple el mínimo de 50% de MODO REMOTO.

### Para activar este lote, pegá esto en LinkedIn y volvé con los resultados

Para cada una de las 8 empresas arriba, corré esta búsqueda y pegá nombre + título + headline de posteo reciente (si tiene):

```
LinkedIn search: "[Empresa]" AND ("Product Manager" OR "PM" OR "Senior PM" OR "Group PM") AND "Argentina" OR "LATAM" OR "Remote"
```

Mix por empresa (para que la asignación de arriba funcione sin ajustes):
- 1-2 PMs a tu nivel (Senior PM / PM)
- 1 PM un nivel arriba (Group PM, Director — posible hiring manager)
- 1 persona de función adyacente (Eng Manager, Design Lead) o reclutador/a regional

### Networking virtual de esta semana (MODO REMOTO)

Unirte a **Product School Slack** y a la **comunidad de Lenny (Lenny's Newsletter community)**, y comentar en 2-3 threads relevantes sobre PM/producto esta semana. Esto no reemplaza el outreach 1:1 de arriba, pero es la acción de red remota de menor fricción disponible hoy sin depender de datos de LinkedIn.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguna.** Revisando las fechas de "Conectado desde" en `rastreador-conexiones.md`, la conexión más reciente registrada es Sharik Garzón Terán (Mercado Libre, 19 Nov 2025) y OGHENETEJIRI Atebefia (Amazon, 17 Feb 2026) — ninguna cae dentro de las últimas 48 horas desde hoy (17 Nov 2026).

**Nota de confiabilidad:** el archivo no se actualizó desde 2026-08-13. Si enviaste solicitudes nuevas en los últimos 3 meses y alguna fue aceptada, no está reflejado acá — convendría revisar manualmente "Mis Conexiones" en LinkedIn ordenado por fecha y actualizar `rastreador-conexiones.md` antes de la próxima corrida para que este chequeo sea confiable.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
**Ninguno generado hoy.** El trigger es "rol postulado en las últimas 48 horas sin referido" — pero Parte 1 de hoy confirma 0 postulaciones enviadas en todo el sistema (100 días, 0 envíos), así que no hay un evento de postulación reciente que dispare un pedido nuevo.

### Recordatorios (5+ días, sin respuesta)
**Ninguno generado hoy.** `rastreador-conexiones.md` no tiene ningún campo de "Referido solicitado" poblado con fecha de envío (no existe tampoco `referral-tracker-template.md` en el repo), así que no hay un pedido de referido real en curso del cual hacer seguimiento.

### Contexto que sí existe (sin acción automática — ya señalado en corridas anteriores)
`rastreador-conexiones.md` identifica 6 contactos de alta prioridad para pedido de referido que siguen sin activarse 96 días después de haberse identificado: Elena Yndurain (Microsoft, Director AI Product Management), Virginia Silvero y Bernardo Manzella (Globant), Melina Ruggeri (Salesforce), Maria Jose Trejo Conde y Pedro Alejandro Santamarina (Mercado Libre). No corresponde generar los mensajes acá porque ninguno cumple el trigger de esta Parte 2 (conexión reciente aceptada o postulación de las últimas 48h) — para generarlos, correr `/pedir-referido [nombre] + [rol]` directamente.

---

## Resumen ejecutivo para el usuario

El cuello de botella de networking no es falta de proceso — es falta de **datos frescos en dos lugares**: (1) `rastreador-conexiones.md` sin tocar en 96 días, y (2) cero perfiles de LinkedIn nuevos disponibles para las 8 empresas remote-friendly con gap. Ambos requieren una acción manual puntual (exportar conexiones nuevas de LinkedIn + correr las 8 búsquedas de arriba) antes de que el sistema pueda generar el próximo lote real de 25 solicitudes. Mientras tanto, los 6 pedidos de referido ya identificados siguen siendo la acción de mayor apalancamiento disponible hoy sin esperar nada más.
