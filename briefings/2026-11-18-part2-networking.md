# Parte 2: Networking - Miércoles, 18 de Noviembre de 2026

**Gate de calidad:** `empresas-objetivo.md` y `plan-carrera.md` tienen datos reales (no placeholders) — OK para continuar. `rastreador-conexiones.md` tiene datos reales pero **su última actualización registrada sigue siendo 2026-08-13 — 97 días sin tocar** (confirmado también por Parte 1 de hoy). El commit más reciente que tocó este archivo es del 2026-11-03 (solo reorganización de briefings, no datos nuevos de LinkedIn). Esto sigue limitando lo que esta corrida puede confirmar con certeza.

**Modo detectado (`plan-carrera.md`):** Función = Product Management (PM/PO, abierto a IC Senior / Lead-Head / especialización IA). Modalidad = **Remoto excluyente** (filtro duro) → se activa **MODO REMOTO**. No aplica Modo Director+/Empleado (el usuario no está empleado actualmente — ver Debilidad 2 del plan de carrera — y el nivel objetivo no es Director+). No aplica Modo Returner (el gap real es de ~1 mes de transición, no un career gap que amerite reactivación de red dormida).

---

## ⚠️ Nuevas Solicitudes de Conexión — mismo bloqueo que ayer, no se fabricaron 25 personas

Sin acceso a LinkedIn en esta sesión desatendida y sin ningún dato nuevo en `rastreador-conexiones.md` desde la última corrida, generar 25 filas con nombres reales sigue siendo imposible sin inventar personas — lo cual el propio skill de `/solicitud-conexion` prohíbe explícitamente. No hay cambio de situación respecto al briefing de ayer (2026-11-17).

### Empresas con gap de cobertura (menos de 4 conexiones en `rastreador-conexiones.md`)

Sin cambios: 99 de 108 empresas objetivo con cero conexiones. Amazon (3), Apple (2), Google (2), Salesforce (2) y Atlassian (1) por debajo del umbral de 4. Solo Globant (16), Mercado Libre (16) y Microsoft (5) están cubiertas.

### Para activar el próximo lote de 25 (MODO REMOTO: ≥50% a empresas remote-friendly)

Mismo bloqueo de datos que ayer. Para desbloquearlo, correr en LinkedIn y pegar los resultados (nombre + título + headline reciente):

```
"[Empresa]" AND ("Product Manager" OR "PM" OR "Senior PM" OR "Group PM") AND ("Argentina" OR "LATAM" OR "Remote")
```

Priorizar estas 8 empresas remote-friendly confirmadas con gap (propuesta de distribución del lote de 25, sin cambios respecto a ayer): Deel (4 — lead de rol activo en Parte 1 de hoy), GitLab (3), Nubank (3), VTEX (3), Kavak (3), Atlassian (3), Shopify (3), Stripe (3).

### Reactivación en empresas con contactos reales existentes (Amazon, Apple, Google, Salesforce, Atlassian)

Estas 5 empresas tienen gap de cobertura pero sí tienen contactos reales ya documentados: Alejandro Medici y OGHENETEJIRI Atebefia (Amazon), Pablo Perez y jason cohen (Apple), Gabriel Sleiman (Google), Melina Ruggeri (Salesforce), Carlos Amilcar Sanchez Rosa (Atlassian). Los mensajes de reactivación de 15 minutos para ellos ya fueron redactados en `briefings/2026-11-16-part2-networking.md` — no se regeneran acá para no duplicar contenido. **Si todavía no se enviaron, siguen siendo la acción de hoy.**

### Networking virtual de esta semana (MODO REMOTO)

Unirte a **Product School Slack** y a la comunidad de **Lenny's Newsletter**, y comentar en 2-3 threads relevantes sobre PM/producto esta semana. Acción de red remota de menor fricción disponible sin depender de datos de LinkedIn.

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

**Ninguna.** La conexión más reciente registrada en `rastreador-conexiones.md` sigue siendo Sharik Garzón Terán (Mercado Libre, 19 Nov 2025) y OGHENETEJIRI Atebefia (Amazon, 17 Feb 2026) — ninguna cae dentro de las últimas 48 horas desde hoy (18 Nov 2026).

**Nota de confiabilidad (sin cambios):** el archivo no se actualizó con datos nuevos desde 2026-08-13. Si se enviaron solicitudes nuevas en los últimos meses y alguna fue aceptada, no está reflejado acá. Conviene revisar "Mis Conexiones" en LinkedIn ordenado por fecha y actualizar `rastreador-conexiones.md` antes de la próxima corrida.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
**Ninguno generado hoy.** El trigger es "rol postulado en las últimas 48 horas sin referido" — Parte 1 de hoy confirma 0 postulaciones enviadas en todo el sistema (101 días, 0 envíos), así que no hay evento de postulación reciente que dispare un pedido nuevo.

### Recordatorios (5+ días, sin respuesta)
**Ninguno generado hoy.** No existe `template-rastreador-referidos.md` poblado con fechas reales de pedidos enviados (el archivo en `plantillas/` sigue siendo el template vacío), así que no hay un pedido de referido real en curso del cual hacer seguimiento.

### Contexto que sí existe (sin acción automática — señalado 98 días consecutivos)
Los mismos 6 contactos de alta prioridad siguen sin activarse: **Elena Yndurain** (Microsoft, Director AI Product Management), **Virginia Silvero** y **Bernardo Manzella** (Globant), **Melina Ruggeri** (Salesforce), **Maria Jose Trejo Conde** y **Pedro Alejandro Santamarina** (Mercado Libre). No corresponde generar los mensajes acá porque ninguno cumple el trigger de esta Parte 2 — para generarlos, correr `/pedir-referido [nombre] + [rol]` directamente.

---

## Resumen ejecutivo para el usuario

Situación sin cambios respecto a ayer: el cuello de botella sigue siendo falta de datos frescos, no falta de proceso. `rastreador-conexiones.md` lleva 97 días sin una actualización real y no hay perfiles de LinkedIn nuevos disponibles para las 8 empresas remote-friendly con gap. Dos acciones manuales puntuales desbloquearían el próximo lote real de 25 solicitudes: (1) exportar conexiones nuevas de LinkedIn, (2) correr las 8 búsquedas de arriba y pegar los resultados. Mientras tanto, los 6 pedidos de referido ya identificados y las 5 reactivaciones de contactos existentes (Amazon/Apple/Google/Salesforce/Atlassian) son la acción de mayor apalancamiento disponible hoy, sin esperar nada más.
