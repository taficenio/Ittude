# Briefing Matutino - Parte 2: Networking
# Solicitudes de conexión, seguimientos, nudges de referidos

> **Configuración de Cowork:** Programar a las 7:15 AM días de semana. Guarda output en `briefings/[AAAA-MM-DD]-part2-networking.md`.
> Esta parte se ejecuta de forma independiente. Lee el output de la Parte 1 si está disponible para contexto de roles.

---

Leer todos los archivos en la carpeta job-search-os/biblioteca-contexto/. También leer job-search-os/CLAUDE.md para las reglas del sistema. Si el output de hoy de la Parte 1 existe en `briefings/[AAAA-MM-DD]-part1-roles.md`, leerlo para contexto de los roles top.

## Gate de Calidad

Verificar que estos archivos contengan datos reales (no placeholders de template):
1. **rastreador-conexiones.md** -- Necesario para seguimientos y nudges de referidos. Si está vacío, el networking se limitará solo a nuevo outreach.
2. **empresas-objetivo.md** -- Necesario para identificar gaps de cobertura. Si está vacío, DETENER y decir: "Completar empresas-objetivo.md primero."
3. **plan-carrera.md** -- Necesario para detección de función y modos de persona. Si está vacío, DETENER y decir: "Completar plan-carrera.md primero."

## Detección del Tipo de Rol

Leer `plan-carrera.md` para detectar la función objetivo del usuario. Apuntar a contactos de networking apropiados para la función.

---

## Nuevas Solicitudes de Conexión

Identificar empresas en empresas-objetivo.md donde el usuario tiene menos de 4 conexiones en rastreador-conexiones.md. Estos son gaps de cobertura.

**Por defecto: 25 solicitudes de conexión**, distribuidas round-robin entre empresas con gaps (no enviar las 25 a una empresa).

**MODO DIRECTOR+ / EMPLEADO:** Si plan-carrera.md muestra Director+ Y actualmente empleado, reducir a 5-10 pedidos. Apuntar solo a pares VP/Director, ejecutivos CPO/SVP contratadores y reclutadores ejecutivos. Proveer justificación estratégica para cada uno. Agregar nota de confidencialidad: "Modo ejecutivo empleado: Todo el outreach enmarcado como networking profesional, no búsqueda de trabajo. Sin señales de 'Open to Work'."

**MODO REMOTO:** Si plan-carrera.md muestra preferencia remota, priorizar empresas remote-friendly (GitLab, Automattic, Zapier, Buffer, y cualquiera marcada en empresas-objetivo.md). Asignar al menos 50% del lote a empresas confirmadas remote-friendly. También sugerir 1-2 comunidades virtuales: PM: Product School Slack, comunidad de Lenny. SWE: servidores de Discord, comunidades open-source. Diseño: ADPList. Formato: "Networking virtual de esta semana: Unirte a [comunidad] y comentar en 2-3 threads relevantes."

**MODO RETURNER:** Si plan-carrera.md muestra un gap de carrera, verificar si el usuario reactivó conexiones dormidas esta semana. Si no: "REACTIVACIÓN DE RED: Enviar 3-5 mensajes a ex-colegas en o cerca de empresas objetivo. Template: 'Hola [Nombre], ¡pasó mucho tiempo! Estoy explorando roles de [función] nuevamente -- me encantaría saber cómo estás. ¿Tendrías chance de ponernos al día rápido?'"

Para cada solicitud de conexión:
- Un mensaje personalizado (300 caracteres máx, límite de LinkedIn)
- Debe incluir: referencia específica al trabajo/background de la persona, un punto de conexión (conexión mutua, escuela compartida, empresa compartida, ubicación, o detalle específico del rol), y el calificador de una línea del usuario
- Tono: cálido, humano, levemente casual. No corporativo. No desesperado.

Output como tabla:
| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|

---

## Seguimientos (Conexiones Aceptadas en las Últimas 48 Horas)

Verificar rastreador-conexiones.md para conexiones que pasaron de "solicitada" a "conectada" en las últimas 48 horas.

Para cada nueva conexión aceptada, redactar un seguimiento:
- Agradecerles por conectar
- Referenciar algo específico sobre su background
- Pedido suave de una conversación de 15 minutos (no un referido -- demasiado pronto)
- Menos de 500 caracteres

---

## Nudges de Referidos (Pedidos Sin Respuesta)

Verificar rastreador-conexiones.md y referral-tracker-template.md para:
- **Pedidos de referido enviados hace 5+ días sin respuesta:** Redactar un recordatorio suave de una sola vez. Corto. Sin presión. Ejemplo: "Hola [Nombre], solo chequeando el referido para el puesto de [Rol]. Totalmente entendible si el timing no funciona -- te lo agradezco de cualquier manera."
- **Roles postulados en las últimas 48 horas sin referido:** Identificar la conexión más cercana en esa empresa y redactar un pedido de referido.

---

## Output

Guardar todo en `job-search-os/briefings/[AAAA-MM-DD]-part2-networking.md` usando este formato:

```markdown
# Parte 2: Networking - [Fecha Completa]

## Solicitudes de Conexión ([N] en total)

| # | Nombre | Empresa | Rol | Mensaje |
|---|------|---------|------|---------|
| 1 | [Nombre] | [Empresa] | [Rol] | [mensaje 300 chars] |
| ... | | | | |

## Seguimientos (Recién Conectados)

### [Nombre] en [Empresa]
Conectado: [fecha]
Mensaje: [borrador del seguimiento]

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido
- [Nombre] para [Rol] en [Empresa]: [borrador del mensaje]

### Recordatorios (5+ días, sin respuesta)
- [Nombre] para [Rol] en [Empresa]: [borrador del recordatorio]
```
