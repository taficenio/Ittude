# Briefing Matutino - Parte 1: Nuevos Roles
# Escanear empresas objetivo, puntuar roles, adaptar CVs para los mejores matches

> **Configuración de Cowork:** Programar a las 7:00 AM días de semana. Guarda output en `briefings/[AAAA-MM-DD]-part1-roles.md`.
> Esta parte se ejecuta de forma independiente. Las Partes 2 y 3 referencian su output.

---

Leer todos los archivos en la carpeta job-search-os/biblioteca-contexto/. También leer job-search-os/CLAUDE.md para las reglas del sistema.

## Gate de Calidad

Antes de ejecutar, verificar que estos archivos contengan datos reales (no placeholders de template como `[COMPLETAR]`):

1. **biblioteca-experiencias.md** -- Si está vacío o solo con placeholders, DETENER. Decir: "Tu biblioteca de experiencias no está completa. Ejecutar `Ayudame a construir mi biblioteca de experiencias` primero."
2. **plan-carrera.md** -- Si está vacío o solo con placeholders, DETENER. Decir: "Tu plan de carrera no está completo. Completar plan-carrera.md primero."
3. **empresas-objetivo.md** -- Si está vacío o solo con placeholders, DETENER. Decir: "Tu lista de empresas objetivo no está completa. Completar empresas-objetivo.md primero."

Si algún check falla, NO continuar.

## Detección del Tipo de Rol

Leer `plan-carrera.md` para detectar la función objetivo del usuario (PM, SWE, Diseño, Data Science, Marketing, CS). Todas las secciones abajo se adaptan a la función detectada. Buscar postulaciones apropiadas para la función, no roles de PM por defecto.

---

## Motivación y Estado

Determinar en qué semana de la búsqueda estamos contando desde la fecha de postulación más temprana en app-tracker (o la fecha de creación del sistema si no hay postulaciones).

**Si app-tracker.md no existe o está vacío:** Armar datos del pipeline desde `empresas-objetivo.md` (campos de Estado, tabla de Resumen por Estado), `rastreador-conexiones.md` (fechas de referidos), `historial-entrevistas.md` (fechas de entrevistas), y carpeta `briefings/` (actividad reciente). Notar: "Stats del pipeline armados desde fuentes alternativas. Para tracking preciso, ejecutar `/rastrear-postulaciones agregar` para cada postulación activa."

Mostrar:
```
Semana [N] de tu búsqueda.
Stats desde el inicio: Postulaciones: [N] | Entrevistas: [N] | Ofertas: [N]
[Una oración de coaching basada en datos -- NO motivación genérica. Basarse en patrones reales.]
```

---

## Escaneo de Nuevos Roles

Buscar en cada empresa de empresas-objetivo.md nuevas postulaciones de la función objetivo del usuario de las últimas 24 horas. Verificar páginas de careers y LinkedIn.

**GATE DE CALIDAD DE DATOS:** Si la búsqueda web no está disponible o devuelve errores para una empresa, saltearla y notar: "[Empresa]: no se pudo verificar -- verificar manualmente." NUNCA fabricar listados de trabajo. Si no se puede encontrar una URL real, no incluirla.

**Priorizar verificar:**
- Empresas donde el usuario tiene conexiones (desde rastreador-conexiones.md)
- Top 20 empresas de empresas-objetivo.md
- Empresas con funding reciente o lanzamientos de producto

**MODO DIRECTOR+ / EMPLEADO:** Si plan-carrera.md muestra nivel Director+ Y actualmente empleado, escanear solo las top 10 empresas y mostrar solo roles puntuando 75+.

**MODO REMOTO:** Si plan-carrera.md muestra preferencia remota, filtrar por roles que mencionan "remoto," "distribuido," o "trabajo desde cualquier lugar." Marcar roles "híbrido" o "presencial" con una ADVERTENCIA antes de puntuar.

## Puntuación y Adaptación

Para cada nuevo rol encontrado:
1. Ejecutar puntuar-oferta (score 1-100 en 5 dimensiones: match de habilidades, fit de seniority, señales culturales, rango de compensación, trayectoria de crecimiento)
2. **Roles puntuando 70+:**
   - Ejecutar adaptar-cv usando biblioteca-experiencias.md como fuente
   - Calcular score de cobertura de keywords (% de requisitos del JD coincidentes)
   - Ejecutar sub-agente revisar-como-reclutador en el CV adaptado
   - Ejecutar sub-agente revisar-como-ats en el CV adaptado
   - Auto-corregir problemas marcados y notar todos los cambios
3. **Roles puntuando 60-69:** Marcar como "Postular solo con referido" y notar qué conexiones podrían referir
4. **Roles por debajo de 60:** Saltear pero registrar que fueron revisados

Mostrar los top 3 roles rankeados por score de fit.

## Tarjetas de Roles Top

Para cada uno de los top 3 roles (puntuando 70+), incluir:

### [Título del Rol] en [Empresa] (Score de Fit: [X]/100)

**Por qué es un strong match:** [Resumen de 2 oraciones destacando dimensiones más fuertes]

**CV Adaptado:**
- Estado: [Generado / Auto-corregido / Necesita revisión manual]
- Cobertura de keywords: [X]% ([N]/[M] requisitos del JD coincidentes)
- Revisión de reclutador: Primera impresión [X]/10, Relevancia [X]/10, Legibilidad [X]/10
- Verificación ATS: [PASA / PASA CON ADVERTENCIAS / NO PASA]
- Gaps: [Requisitos del JD no coincidentes por la biblioteca de experiencias]
- Cambios de auto-corrección: [lista de cambios específicos]

**Camino de Referido:**
- Conexión más cercana: [Nombre] en [Empresa] ([solidez de la relación])
- Borrador del mensaje de referido: [mensaje personalizado listo para enviar]
- Sin conexión: "Sin conexión existente. Agregar a prioridad de networking para esta semana."

**Prompt de Trabajo Muestra:**
Prompt apropiado para la función para `/trabajo-muestra`:
```
/trabajo-muestra [Empresa] [Título del Rol] para-conseguir-entrevista
```
Hooks de research:
- [Cosa específica a investigar sobre el producto de esta empresa]
- [Evento reciente o lanzamiento específico a referenciar]
- [Queja específica de usuario o dinámica de mercado a analizar]

---

## Output

Guardar todo en `job-search-os/briefings/[AAAA-MM-DD]-part1-roles.md` usando este formato:

```markdown
# Parte 1: Roles - [Fecha Completa, ej: Lunes, 4 de Mayo de 2026]

## Semana [N] | [Línea de coaching]

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
- [Empresa]: no se pudo verificar -- verificar manualmente
```
