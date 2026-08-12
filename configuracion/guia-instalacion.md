# Guía de Instalación

## Antes de Empezar

**Necesitás una suscripción a Claude.** Claude Pro ($20/mes) o Claude Max ($100-200/mes) en [claude.ai](https://claude.ai). El Buscador de Ofertas ITtude es el sistema; Claude es el motor que lo hace funcionar. La suscripción a Claude es separada y necesaria.

**¿Nunca usaste una terminal?** Sin problema. Ver `terminal-basics.md` en esta carpeta — es una lectura de 2 minutos que cubre todo lo que necesitás. No se requiere saber programar. Vas a escribir en español y pegar descripciones de puestos.

**¿Usás Windows?** La mayoría de usuarios LATAM usan Windows. Tenés dos opciones:
- **Opción A (más sencilla):** Instalar WSL (Windows Subsystem for Linux). Abrí PowerShell como administrador y ejecutá: `wsl --install`. Reiniciá. Luego seguí todos los pasos abajo dentro de tu terminal WSL.
- **Opción B:** Usar directamente PowerShell o Git Bash en Windows. Claude Code también funciona en Windows nativo.

## Paso 1: Instalar Claude Code

**Mac / Linux / WSL:**
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

**Windows (PowerShell como administrador):**
```powershell
winget install Anthropic.ClaudeCode
```

Verificar que funciona:
```bash
claude --version
```

## Paso 2: Abrir el Proyecto en tu Editor

1. Descargá o descomprimí la carpeta del proyecto
2. Abrí Cursor > Archivo > Abrir Carpeta > seleccionar la carpeta `job-search-os`
3. Configurar layout de tres paneles: árbol de archivos (izquierda), editor (centro), terminal (abajo)

También funciona con VS Code u otro editor con terminal integrada.

## Paso 3: Iniciar Claude Code

En la terminal del editor:
```bash
claude
```

Claude lee automáticamente `CLAUDE.md` y entiende todo el sistema.

## Paso 4: Explorar el Sistema

```
Leer CLAUDE.md y resumir qué hace este Buscador de Ofertas ITtude
```

Navegar por las carpetas. Click derecho en cualquier archivo `.md` > Abrir Vista Previa para leerlo formateado.

## Paso 5: Construir tu Biblioteca de Experiencias (~30 min)

```
Ayudame a construir mi biblioteca de experiencias
```

Pegá tu CV Y tu perfil de LinkedIn (copiá el texto o exportalo). Claude combina ambos, elimina duplicados y organiza por categoría de habilidad. Luego pregunta sobre proyectos que ninguna fuente captura.

Tip: Usá dictado en lugar de escribir. 30 min hablando produce una biblioteca más rica que 1 hora escribiendo.

Este es el paso más importante. Si tu biblioteca de experiencias está vacía, todo lo que produce el OS será genérico. Si está rica, todo es quirúrgico.

## Paso 6: Completar el Doc de Q&A Maestro

```
Ayudame a completar el doc de Q&A maestro
```

Claude te guía por la estrategia de compensación, preguntas comunes de postulación y logística. Completar una vez, usado en todas partes.

## Paso 7: Crear tu Plan de Carrera

```
Ayudame a completar mi plan de carrera
```

Rankear tus preferencias (nivel, industria, función). Claude identifica tus debilidades comparando tu CV contra JDs típicos. El análisis de direccionamiento de debilidades orienta todo: posicionamiento del CV, "contame sobre vos" y prep de entrevista.

Gastar 15 minutos en la sección de debilidades. Son los 15 minutos de más alto leverage en todo el setup.

## Paso 8: Generar Empresas Objetivo

```
/investigar-empresa generar lista de targets
```

Describí tus empresas ideales en 2-3 oraciones. Claude genera ~100 entradas. Revisar, editar y reordenar.

## Paso 9: Configurar el Briefing Matutino

Ver `morning-briefing-setup.md` para la configuración exacta de Cowork.

## Paso 10: Configurar Grabación de Entrevistas (Opcional)

Granola (granola.ai) es una herramienta de transcripción de reuniones que graba y transcribe entrevistas automáticamente. Si no usás Granola, podés pegar manualmente transcripciones de entrevistas en `/debrief-entrevista` después de cada entrevista.

## Paso 11: Primera Ejecución Manual

Antes de confiar en la automatización, ejecutar el briefing manualmente:

```
Leer tareas-cowork/daily-morning-briefing.md y ejecutarlo
```

Revisar el output. ¿Son relevantes los roles? ¿Son buenos los CVs? Ajustar los archivos de contexto si algo está mal. Confiar en la automatización después de 2-3 buenas ejecuciones.

## Prerequisitos y Costos

- **Suscripción Claude Pro** ($20/mes) es necesaria para correr Claude Code. El sistema es una compra única; Claude Pro es tu runtime.
- **Cursor** (tier gratuito funciona). Cualquier editor con terminal funciona, pero el layout de tres paneles de Cursor es ideal.
- **Cowork** (opcional, tier gratuito disponible). Solo necesario para el briefing matutino automatizado. Los 18 skills funcionan en modo standalone en Claude Code sin Cowork.
- **Granola** (opcional, tier gratuito disponible). Solo necesario para transcripción automática de entrevistas.

## Solución de Problemas

**"claude: command not found"**
Cerrar y volver a abrir la terminal después de instalar. Si sigue sin funcionar: `export PATH="$HOME/.claude/bin:$PATH"` y luego ejecutar `claude` de nuevo. En Windows, usar WSL2.

**"Permission denied" durante la instalación**
Ejecutar con privilegios de admin: `sudo curl -fsSL https://claude.ai/install.sh | bash`

**Claude Code inicia pero no lee CLAUDE.md**
Asegurarse de abrir la carpeta `job-search-os` directamente en Cursor (no una carpeta padre). Claude Code lee CLAUDE.md desde el directorio de trabajo actual.

**CVs genéricos / output de baja calidad**
Tu biblioteca de experiencias está demasiado delgada. Esta es la causa #1 de output pobre. Volver al Paso 5 y agregar más detalle. Apuntar a 12+ historias STAR en el banco de historias y métricas detalladas en cada bullet.

**"No soy PM — ¿funcionará para mí?"**
El sistema está optimizado para roles de PM pero el motor central (adaptación de CV, networking, prep de entrevista, negociación) funciona para cualquier rol de trabajador del conocimiento. Los datos insider y los frameworks de entrevista son específicos de PM. Si estás en ingeniería, diseño, marketing u otras funciones, los skills igualmente corren — solo salteá los datos insider específicos de PM.

**"Estoy en Argentina/México/Colombia y busco trabajo remoto"**
¡Perfecto! El sistema está optimizado para esto. Las fuentes de investigación salarial incluyen GetOnBoard, Computrabajo, SysArmy y Glassdoor LATAM para roles locales. Para roles remotos globales con pago en USD, también usa levels.fyi y Glassdoor global. La base de datos de company-intel incluye empresas LATAM (Mercado Libre, Rappi, Nubank, etc.) y empresas globales que contratan en LATAM.

**El briefing matutino no ejecuta automáticamente**
Tu computadora debe estar encendida y Claude Desktop debe estar abierto a la hora programada. Si usás laptop, verificar configuración de suspensión. Considerar programar 30 min después de tu alarma.

**Company intel parece desactualizado**
Los datos insider fueron vigentes a la fecha de construcción del OS. Para cualquier empresa, ejecutar `/investigar-empresa [empresa]` para obtener datos frescos de la web. El intel precargado es un punto de partida — siempre complementar con research actualizado antes de entrevistas.

**Los skills producen errores o output incompleto**
Ejecutar `/clear` y volver a intentar. Las conversaciones largas degradan el contexto de Claude. Empezar de cero entre tareas no relacionadas. Si un skill falla consistentemente, verificar que los archivos de biblioteca-contexto requeridos estén completos (no solo placeholders de template).
