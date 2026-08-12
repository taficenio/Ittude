# Actualizar el Buscador de Ofertas ITtude

Cuando se lanza una nueva versión, seguir estos pasos para actualizar sin perder tus datos personales.

## Proceso de Actualización

1. **Descargar la nueva versión** de la fuente de distribución.
2. **Copiar estas carpetas y archivos** de la nueva versión a tu carpeta `job-search-os` existente, reemplazando las versiones viejas:
   - `.claude/skills/` (todos los archivos de skills)
   - `sub-agentes/` (todos los archivos de sub-agentes)
   - `datos-insider/` (perfiles de company intel y frameworks)
   - `tareas-cowork/` (prompts de tareas programadas)
   - `plantillas/` (archivos de templates)
   - `CLAUDE.md` (archivo de configuración raíz)
3. **NO sobreescribir `biblioteca-contexto/`.** Esta carpeta contiene tus datos personales (biblioteca de experiencias, plan de carrera, empresas objetivo, tracker de conexiones, historial de entrevistas, etc.). Se mantiene intacta durante las actualizaciones.
4. **Verificar el número de versión en `CLAUDE.md`** después de copiar para confirmar que la actualización se aplicó correctamente.

## Qué se Actualiza vs. Qué se Preserva

| Actualizado (reemplazar con nueva versión) | Preservado (nunca sobreescribir) |
|---------------------------------------------|----------------------------------|
| `.claude/skills/` | `biblioteca-contexto/` |
| `sub-agentes/` | `briefings/` |
| `datos-insider/` | Cualquier nota o archivo personal que hayas agregado |
| `tareas-cowork/` | |
| `plantillas/` | |
| `CLAUDE.md` | |

## Si Algo Se Rompe

Si una actualización causa problemas, verificar el `CHANGELOG.md` en la raíz del proyecto para ver qué cambió en cada versión. Si un skill se comporta diferente, el changelog notará los breaking changes.
