# Conceptos Básicos de Terminal (Orientación de 2 minutos)

## ¿Qué es una terminal?

Una terminal es una ventana de texto donde escribís comandos y presionás Enter. Pensala como enviarle mensajes de texto a tu computadora en lugar de hacer clic en botones. Escribís algo, presionás Enter, y te responde.

## Cómo abrir una terminal

**Mac:**
- Abrir Spotlight (Cmd + Space), escribir "Terminal", presionar Enter
- O ir a Aplicaciones > Utilidades > Terminal

**Windows:**
- Presionar la tecla Windows, escribir "Símbolo del sistema" o "PowerShell", presionar Enter
- O presionar Win + R, escribir `cmd`, presionar Enter
- **Recomendado para Windows:** Instalar WSL y usar la terminal de Ubuntu (ver installation-guide.md)

## Qué pasa cuando escribís `claude`

Una vez que Claude Code está instalado, escribir `claude` y presionar Enter inicia una conversación interactiva. Vas a ver un prompt donde podés escribir en español — cosas como "Ayudame a construir mi biblioteca de experiencias" o pegar una descripción de puesto. No se necesitan conocimientos de programación.

## ¿Qué son los archivos .md?

Los archivos que terminan en `.md` son archivos Markdown — solo texto plano con formato simple (como `#` para títulos y `**negrita**` para texto en negrita). Podés leerlos y editarlos en cualquier editor de texto.

**Para leerlos con buen formato:**
- En Cursor o VS Code: click derecho en el archivo > "Abrir Vista Previa"
- En GitHub: se muestran formateados automáticamente
- En cualquier editor de texto: son perfectamente legibles como texto plano también

## Navegar a la carpeta del Buscador de Ofertas ITtude

Antes de escribir `claude`, necesitás estar en la carpeta correcta:

- **La forma más fácil:** Escribir `cd ` (con un espacio después), luego arrastrar la carpeta `job-search-os` desde el Explorador de archivos (Windows) o Finder (Mac) a la ventana de la terminal. Presionar Enter.
- **O escribir la ruta directamente:** `cd C:\Users\TuNombre\Documents\job-search-os` en Windows, o `cd ~/Documents/job-search-os` en Mac/Linux.

**Con Cursor/VS Code:** No necesitás hacer esto. Cuando abrís la carpeta en el editor, la terminal ya está en esa carpeta.

## Eso es todo

Ahora sabés suficiente para usar el Buscador de Ofertas ITtude. Abrir tu editor, iniciar Claude Code en la terminal, y seguir START-HERE.md.
