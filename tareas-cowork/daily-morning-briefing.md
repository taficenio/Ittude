# Briefing Matutino Diario de Búsqueda Laboral (Archivo Maestro)

Este briefing está dividido en 3 partes independientes para ajustarse dentro de los límites de contexto de Claude. Cada parte puede ejecutarse de forma independiente.

## Estructura de 3 Partes

| Parte | Archivo | Alcance | Output |
|------|------|-------|--------|
| **Parte 1: Roles** | `briefing-part1-roles.md` | Escanear empresas objetivo, puntuar roles, adaptar CVs | `briefings/[fecha]-part1-roles.md` |
| **Parte 2: Networking** | `briefing-part2-networking.md` | Solicitudes de conexión, seguimientos, nudges de referidos | `briefings/[fecha]-part2-networking.md` |
| **Parte 3: Coaching** | `briefing-part3-coaching.md` | Salud del pipeline, coaching de entrevistas, stack de prioridades | `briefings/[fecha]-part3-coaching.md` |

## Para Cowork: Programar Parte 1 a las 7:00 AM, Parte 2 a las 7:15 AM, Parte 3 a las 7:30 AM. O ejecutar las 3 secuencialmente en una sesión.

**Configuración:**
- Nombrar cada tarea: "Briefing de Búsqueda - Parte [N]"
- Cadencia: Días de semana
- Pegar el contenido de cada archivo de parte como el prompt de la tarea programada.
- La Parte 3 lee el output de las Partes 1 y 2, así que debe ejecutarse última.

**Ejecución manual:**
- Pegar cualquier archivo de parte individual en Claude Code para ejecutarlo.
- O ejecutar los 3 en orden para un briefing completo.

Ver `configuracion/setup-briefing-matutino.md` para instrucciones detalladas de configuración.

---

# Briefing Completo (Referencia de Sesión Única)

> Para usuarios con Claude Max que quieran ejecutar el briefing completo en una sola sesión, pegar todo debajo de la línea como un único prompt. Este es el briefing original no abreviado.

> **Uso de tokens:** Con Claude Pro, usar la división en 3 partes de arriba. Si el briefing se corta, volver a ejecutar con "Continuar desde la Parte [N]." Claude Max provee límites más altos para ejecuciones de briefing completo.

---

# Briefing Matutino - Buscador de Ofertas ITtude

Leer todos los archivos en la carpeta job-search-os/biblioteca-contexto/. También leer job-search-os/CLAUDE.md para las reglas del sistema.

## GATE DE CALIDAD -- Verificación de Contexto Requerida

Antes de ejecutar cualquier parte del briefing, verificar que estos tres archivos estén completos con datos reales (no solo placeholders de template):

1. **biblioteca-experiencias.md** -- Si este archivo está vacío o contiene placeholders de template (ej: corchetes como "[bullet con métrica específica...]"), DETENER. Decirle al usuario: "Tu biblioteca de experiencias no está completa. El briefing matutino depende de ella para la adaptación de CVs y el puntaje de fit. Ejecutar `Ayudame a construir mi biblioteca de experiencias` primero, luego volver a ejecutar el briefing."
2. **plan-carrera.md** -- Si este archivo está vacío o contiene solo placeholders de template, DETENER. Decirle al usuario: "Tu plan de carrera no está completo. El briefing lo usa para puntuar el fit y posicionamiento. Completar plan-carrera.md primero, luego volver a ejecutar el briefing."
3. **empresas-objetivo.md** -- Si este archivo está vacío o contiene solo placeholders de template, DETENER. Decirle al usuario: "Tu lista de empresas objetivo no está completa. El briefing escanea estas empresas para nuevos roles. Completar empresas-objetivo.md primero, luego volver a ejecutar el briefing."

Si alguno de los tres checks falla, NO continuar. El briefing producirá output de baja calidad o inútil sin estos archivos.

## Detección del Tipo de Rol

Leer `plan-carrera.md` para detectar la función objetivo del usuario (PM, SWE, Diseño, Data Science, Marketing, CS). Todas las secciones abajo se adaptan basándose en la función detectada:
- Parte 1: Buscar postulaciones apropiadas para la función (no "postulaciones de PM/producto" para usuarios no-PM)
- Parte 2: Apuntar a contactos de networking apropiados para la función
- Parte 3: Generar prompts de trabajo muestra apropiados para la función
- Salud del Pipeline: Usar benchmarks y recomendaciones de drill apropiados para la función
- Coaching de Entrevista: Referenciar tipos de mock y categorías de preguntas apropiados para la función

---

Antes de cualquier otra cosa, calcular y mostrar:

## Motivación y Estado

Determinar en qué semana de la búsqueda laboral estamos contando desde la fecha de postulación más temprana en app-tracker (o la fecha de creación del sistema si no hay postulaciones aún).

**Si app-tracker.md no existe o está vacío:** Armar datos del pipeline desde fuentes alternativas:
- Desde `empresas-objetivo.md`: Escanear campos de Estado (ej: "EN PROCESO", "REFERIDO ENVIADO", "SIN EMPEZAR") y la tabla de Resumen por Estado.
- Desde `rastreador-conexiones.md`: Extraer fechas de referidos y actividad reciente.
- Desde `historial-entrevistas.md`: Extraer fechas de entrevistas y empresas.
- Desde la carpeta `briefings/`: Verificar archivos de briefing recientes para actividad registrada.
- Usar estos para estimar conteo de postulaciones, entrevistas y estado del pipeline. Notar en el output: "Stats del pipeline armados desde empresas-objetivo.md e historial-entrevistas.md (no se encontró app-tracker.md). Para tracking preciso, ejecutar `/rastrear-postulaciones agregar` para cada postulación activa."

```
Semana [N] de tu búsqueda.

Stats desde el inicio:
- Postulaciones enviadas: [N]
- Entrevistas completadas: [N]
- Ofertas recibidas: [N]

[Una oración de coaching contextual. NO motivación genérica. Basarse en patrones de datos reales. Ejemplos:
- Si la tasa de respuesta está subiendo: "Tu tasa de respuesta mejoró de X% a Y% en las últimas 2 semanas. Los cambios de targeting están funcionando."
- Si el volumen de entrevistas está subiendo: "3 entrevistas esta semana vs 1 la semana pasada. La inversión en networking está dando resultados."
- Si es temprano y el volumen es bajo: "Semana 2. El volumen es bajo pero es esperado. La prioridad ahora es construir tu red de referidos, no postular masivamente."
- Si hubo un rechazo: "[Empresa] no avanzó, pero tus puntajes de entrevista promediaron 7.2/10. La performance está ahí -- seguí adelante."
- Si la búsqueda lleva mucho tiempo: "Semana 8. Las búsquedas largas ponen a prueba la paciencia. Tu tasa de conversión está en realidad por encima del benchmark. Mantené el sistema funcionando."
]
```

---

## Parte 1: Nuevos Roles

Buscar en cada empresa de empresas-objetivo.md nuevas postulaciones del tipo de rol del usuario de las últimas 24 horas. Verificar sus páginas de careers y LinkedIn.

**[ADAPTATIVO-POR-FUNCIÓN]** Buscar postulaciones de la función objetivo del usuario, no solo postulaciones de PM.

### GATE DE CALIDAD DE DATOS
Si la búsqueda web no está disponible o devuelve errores para alguna empresa, saltear esa empresa y notarlo en el output como "[Empresa]: no se pudo verificar -- verificar manualmente." NUNCA fabricar listados de trabajo. Si no se puede encontrar una URL real para un rol, no incluirlo.

Priorizar verificar:
- Empresas donde el usuario tiene conexiones (desde rastreador-conexiones.md) -- estas tienen la tasa de conversión más alta
- Empresas en el top 20 de empresas-objetivo.md
- Empresas con rondas de funding o lanzamientos de producto recientes

Para cada nuevo rol encontrado:
1. Ejecutar el proceso de puntuar-oferta (score 1-100 en 5 dimensiones: match de habilidades, fit de seniority, señales culturales, rango de compensación, trayectoria de crecimiento)
2. Para roles puntuando 70+:
   - Ejecutar el proceso de adaptar-cv usando biblioteca-experiencias.md como fuente
   - Calcular score de cobertura de keywords (% de requisitos del JD coincidentes)
   - Ejecutar el sub-agente revisar-como-reclutador en el CV adaptado
   - Ejecutar el sub-agente revisar-como-ats en el CV adaptado
   - Auto-corregir problemas marcados por los sub-agentes
   - Notar todos los cambios hechos durante la auto-corrección
3. Para roles puntuando 60-69: marcar como "Postular solo con referido" y notar qué conexiones podrían referir
4. Para roles por debajo de 60: saltear pero registrar que fueron revisados

Mostrar los top 3 roles en el briefing, rankeados por score de fit.

---

## Parte 2: Networking

Leer rastreador-conexiones.md y empresas-objetivo.md.

### Nuevas Solicitudes de Conexión (25 en total)

Identificar empresas en empresas-objetivo.md donde el usuario tiene menos de 4 conexiones registradas en rastreador-conexiones.md. Estos son gaps de cobertura.

Generar 25 solicitudes de conexión, distribuidas round-robin entre empresas con gaps (no enviar las 25 a una sola empresa).

Para cada persona:
- Un mensaje personalizado (300 caracteres máx, límite de LinkedIn)
- Debe incluir: una referencia específica al trabajo/background de la persona, un punto de conexión (conexión mutua, escuela compartida, empresa compartida, ubicación, o algo específico sobre su rol), y el calificador de una línea del usuario
- Tono: cálido, humano, levemente casual. No corporativo. No desesperado.

### Seguimientos (conexiones aceptadas en las últimas 48 horas)

Verificar rastreador-conexiones.md para conexiones que pasaron de "solicitada" a "conectada" en las últimas 48 horas.

Para cada nueva conexión aceptada, redactar un mensaje de seguimiento:
- Agradecerles por conectar
- Referenciar algo específico sobre su background
- Pedido suave de una conversación de 15 minutos (no un referido -- demasiado pronto)
- Menos de 500 caracteres

### Nudges de Referidos (pedidos sin respuesta)

Verificar rastreador-conexiones.md y referral-tracker-template.md para:
- Pedidos de referido enviados hace 5+ días sin respuesta: redactar un recordatorio suave de una sola vez
- Roles postulados en las últimas 48 horas sin referido: identificar la conexión más cercana en esa empresa y redactar un pedido de referido

Para los recordatorios:
- Un solo mensaje. Corto. Sin presión.
- Ejemplo: "Hola [Nombre], solo chequeando el referido para el puesto de [Rol]. Totalmente entendible si el timing no funciona -- te lo agradezco de cualquier manera."

---

## Parte 3: Para los Roles Top

Para cada uno de los top 3 roles de la Parte 1 (puntuando 70+), incluir:

### [Título del Rol] en [Empresa] (Score de Fit: [X]/100)

**Por qué es un strong match:**
[Resumen de 2 oraciones sobre por qué este rol puntuó alto, destacando las dimensiones más fuertes]

**CV Adaptado:**
- Estado: [Generado / Auto-corregido / Necesita revisión manual]
- Cobertura de keywords: [X]% ([N]/[M] requisitos del JD coincidentes)
- Revisión de reclutador: Primera impresión [X]/10, Relevancia [X]/10, Legibilidad [X]/10
- Verificación ATS: [PASA / PASA CON ADVERTENCIAS / NO PASA]
- Gaps identificados: [listar requisitos del JD no coincidentes por la biblioteca de experiencias]
- Cambios hechos durante auto-corrección: [listar cambios específicos]

**Camino de Referido:**
- Conexión más cercana: [Nombre] en [Empresa] ([solidez de la relación])
- Borrador del mensaje de referido: [mensaje personalizado listo para enviar]
- Si no hay conexión: "Sin conexión existente. Agregar a prioridad de networking para esta semana."

**Prompt de Trabajo Muestra:**
Prompt listo para usar para `/trabajo-muestra`:
```
/trabajo-muestra [Empresa] [Título del Rol] para-conseguir-entrevista
```
Hooks de research para investigar antes de escribir:
- [Cosa específica a investigar sobre el producto de esta empresa]
- [Evento reciente o lanzamiento específico a referenciar]
- [Queja específica de usuario o dinámica de mercado a analizar]

---

## Output

Guardar todo en job-search-os/briefings/[AAAA-MM-DD]-briefing.md

Usar este formato exacto para el archivo guardado:

```markdown
# Briefing Matutino - [Fecha Completa, ej: Lunes, 4 de Mayo de 2026]

## Semana [N] | [Línea de coaching motivacional de arriba]

---

## Roles Top Hoy

### 1. [Título del Rol] en [Empresa] (Fit: [score]/100)
[Resumen de match de 2 oraciones]
**CV:** [estado + score de cobertura]
**Referido:** [nombre de la conexión + borrador del mensaje O "Sin conexión -- hacer networking primero"]
**Prompt de trabajo muestra:** `/trabajo-muestra [Empresa] [Rol] para-conseguir-entrevista`
**Hooks de research:** [lista con bullets]

### 2. [Título del Rol] en [Empresa] (Fit: [score]/100)
[Misma estructura]

### 3. [Título del Rol] en [Empresa] (Fit: [score]/100)
[Misma estructura]

### Otros Roles Revisados
- [Empresa] [Rol] - Fit: [score] - [SALTEAR / POSTULAR SOLO CON REFERIDO]

### Fallas de Búsqueda
Empresas que no pudieron verificarse (búsqueda web no disponible o errores):
- [Empresa]: no se pudo verificar -- verificar manualmente

---

## Networking a Hacer (25 Solicitudes de Conexión)

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | [Nombre] | [Empresa] | [Rol] | [mensaje 300 chars] |
| ... | | | | |
| 25 | [Nombre] | [Empresa] | [Rol] | [mensaje 300 chars] |

---

## Seguimientos (Conexiones Aceptadas Recientemente)

### [Nombre] en [Empresa]
Conectado: [fecha]
Mensaje: [borrador del seguimiento]

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
- [Nombre] para [Rol] en [Empresa]: [borrador del mensaje]

### Recordatorios (5+ días, sin respuesta)
- [Nombre] para [Rol] en [Empresa]: [borrador del recordatorio]

---

## Resumen del Pipeline

| Etapa | Cantidad | Detalles |
|---|---|---|
| Postulado (esperando) | [N] | Más antigua: [Empresa] ([N] días) |
| Referido solicitado | [N] | |
| Entrevista programada | [N] | Próxima: [Empresa] el [fecha] |
| Entrevistado (esperando resultado) | [N] | |
| Etapa de oferta | [N] | |
| Rechazado esta semana | [N] | |

**Total de postulaciones activas:** [N]
**Entrevistas esta semana:** [N]

---

## Verificación de Salud del Pipeline

[Análisis de cuello de botella basado en datos del pipeline]

---

## Coaching de Debilidades de Entrevista

[Drills y prep urgente basados en historial de entrevistas]

---

## Stack de Prioridades de Hoy

1. [Acción de mayor prioridad con instrucción específica]
2. [Segunda prioridad]
3. [Tercera prioridad]
4. [Si hay tiempo]

Tiempo estimado: [X] minutos total
```
