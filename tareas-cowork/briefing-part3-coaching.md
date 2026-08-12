# Briefing Matutino - Parte 3: Pipeline y Coaching
# Salud del pipeline, coaching de entrevistas, stack de prioridades

> **Configuración de Cowork:** Programar a las 7:30 AM días de semana. Guarda output en `briefings/[AAAA-MM-DD]-part3-coaching.md`.
> Esta parte lee los outputs de hoy de las Partes 1 y 2 para contexto completo.

---

Leer todos los archivos en la carpeta job-search-os/biblioteca-contexto/. También leer job-search-os/CLAUDE.md para las reglas del sistema. Leer los outputs de hoy: `briefings/[AAAA-MM-DD]-part1-roles.md` y `briefings/[AAAA-MM-DD]-part2-networking.md`.

## Gate de Calidad

Verificar que estos archivos contengan datos reales (no placeholders de template):
1. **plan-carrera.md** -- Requerido para detección de persona y coaching. Si está vacío, DETENER.
2. **historial-entrevistas.md** -- Necesario para coaching de debilidades. Si está vacío, saltear esa sección.
3. **app-tracker.md** o fuentes alternativas (`empresas-objetivo.md`, `rastreador-conexiones.md`) -- Necesario para resumen del pipeline.

Leer `plan-carrera.md` para detectar la función objetivo del usuario. Los benchmarks del pipeline y drills se adaptan a la función.

---

## Resumen del Pipeline

Construir desde app-tracker.md (o armar desde empresas-objetivo.md, rastreador-conexiones.md, historial-entrevistas.md, briefings/).

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

Analizar el pipeline y marcar el único cuello de botella más grande:

- **Alto volumen, sin referidos** (postulaciones > 10, referidos = 0): "TU CUELLO DE BOTELLA: Referidos. Postulaciones en frío tienen 3-5% de tasa de respuesta vs 15-25% con referidos. Enfocarse en networking. No más postulaciones en frío sin camino de referido."
- **Referidos no convierten** (referidos > 5, entrevistas = 0): "TU CUELLO DE BOTELLA: CV/Posicionamiento. Los referidos entran pero no convierten a entrevistas. Revisar scores de cobertura. Ejecutar `/auditar-linkedin`."
- **Entrevistas sin prep** (entrevistas > 2 esta semana, sin `/preparar-entrevista` ejecutado): "TU CUELLO DE BOTELLA: Preparación. [N] entrevistas sin paquetes de prep. Ejecutar `/preparar-entrevista` para cada una antes de cualquier otra cosa."
- **Cero volumen** (0 postulaciones esta semana): "TU CUELLO DE BOTELLA: Volumen. Sin postulaciones aún esta semana. Enviar al menos 2 hoy. Si no hay roles 70+, expandir la lista de targets o ajustar criteria en plan-carrera.md."
- **Carrera temprana, semanas iniciales** (< 3 años exp Y semanas 1-4): "RITMO CARRERA TEMPRANA: Priorizar cobertura de referidos sobre volumen. 3-5 postulaciones de calidad por semana con caminos de referido. Crear 1 trabajo muestra esta semana."
- **Pipeline saludable** (postulaciones estables, tasa de referidos > 40%, entrevistas convirtiendo): "Pipeline saludable. [N] postulaciones, [X]% tasa de referidos, [N] entrevistas. Enfocarse en: [acción más impactante basada en estado del pipeline]."

---

## Coaching de Persona Específico

### Candidato Remoto
Si plan-carrera.md muestra preferencia remota: revisar el escaneo de roles de la Parte 1 para advertencias de híbrido/presencial. Confirmar que la Parte 2 priorizó empresas remote-friendly.

### Career Returner
Si plan-carrera.md muestra un gap de carrera:
- **Programas de retorno al trabajo:** Buscar programas activos de returnship en empresas objetivo (Path Forward, iRelaunch, programas específicos de empresas). Reportar hallazgos o sugerir empresas con programas conocidos.
- **Seguimiento de narrativa del gap:** Si historial-entrevistas.md muestra que se preguntó sobre el gap, reportar puntajes y coaching: "Si está mejorando: 'La respuesta del gap se está afinando.' Si no: 'Ejecutar `/simular-entrevista conductual` -- objetivo menos de 45 segundos, mirando hacia adelante, sin sobre-justificación.'"

### Director+ / Empleado
Si Director+ Y actualmente empleado:
- Condensar stack de prioridades a bloque matutino de 60-90 minutos: (1) responder a conversaciones activas, (2) enviar 3-5 pedidos de alta calidad, (3) revisar nuevos roles en top 10, (4) avanzar un trabajo muestra. Todo lo demás para el fin de semana.
- Nota de confidencialidad al inicio del output.

### Founder a Empleado
Si founder/CEO en empresa cerrada:
- **Drill de narrativa de founder:** "Practicar historia de founder de 30 segundos. Liderar con [Marca Fuerte], luego: qué construiste, qué aprendiste, por qué ESTE rol. Tomarte el tiempo -- cortá el medio si supera los 30 segundos."
- **Advertencia de ancla de compensación:** "Tu salario como founder fue $[X]. La tasa de mercado es $[Y]. NO revelar compensación de founder. Usar el encuadre de tasa de mercado de qa-master.md."
- **Prep de señal de estabilidad:** "Ensayar una historia donde diferiste al juicio de alguien más o apoyaste la visión de otro líder."

---

## Coaching de Debilidades de Entrevista

Leer `historial-entrevistas.md` para patrones de debilidades documentados. Si algún tipo de pregunta promedia 6/10 o menos:

- "BRECHA DE HABILIDAD: [Tipo de pregunta] promediando [X]/10. Drill de hoy: Ejecutar `/simular-entrevista [tipo]` y practicar [pregunta específica] hasta puntuar 7+. Tiempo estimado: 30 minutos."

- Si hay entrevistas programadas esta semana que coinciden con una debilidad: "PREP URGENTE: [tipo de entrevista] en [Empresa] esta semana, y el puntaje de [debilidad] es [X]/10. Ejecutar `/preparar-entrevista [Empresa]` y `/simular-entrevista [tipo]` antes de la entrevista. Acción de mayor prioridad hoy."

- Si hay menos de 3 entrevistas registradas, saltear esta sección.

---

## Stack de Prioridades de Hoy

Basándose en la verificación de salud del pipeline, coaching de persona y coaching de debilidades de entrevista, generar el orden de prioridades:

1. [Acción de mayor prioridad con instrucción específica]
2. [Segunda prioridad]
3. [Tercera prioridad]
4. [Si hay tiempo]

Tiempo estimado: [X] minutos total

**MODO DIRECTOR+ / EMPLEADO:** Limitar a 60-90 minutos. Estructurar para un bloque matutino enfocado.

---

## Output

Guardar todo en `job-search-os/briefings/[AAAA-MM-DD]-part3-coaching.md` usando este formato:

```markdown
# Parte 3: Pipeline y Coaching - [Fecha Completa]

## Resumen del Pipeline
[Tabla del pipeline]

## Verificación de Salud del Pipeline
[Análisis del cuello de botella]

## Coaching de Persona
[Cualquier sección de persona aplicable]

## Coaching de Debilidades de Entrevista
[Drills y prep urgente]

## Stack de Prioridades de Hoy
1. [Acción]
2. [Acción]
3. [Acción]
4. [Si hay tiempo]

Tiempo estimado: [X] minutos
```
