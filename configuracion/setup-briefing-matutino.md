# Configuración del Briefing Matutino

El briefing matutino diario es el núcleo del sistema. Escanea nuevos roles, los puntúa, adapta CVs, genera outreach y te da coaching sobre tu pipeline. Así es cómo configurarlo.

## ¿Qué es Cowork?

Cowork es la función de programación de tareas integrada en Claude Desktop. Ejecuta tareas automáticamente según un horario (como un briefing matutino diario). Requisitos:
- App Claude Desktop (no solo el CLI de terminal)
- Suscripción Claude Pro o Max

Si estás ejecutando Claude Code en una terminal sin Claude Desktop, Cowork no está disponible -- usar la Opción 2 (Ejecución Manual) en su lugar. Los 18 skills funcionan sin Cowork.

## Opción 1: Tarea Programada en Cowork (Recomendado)

1. Abrir Cowork
2. Escribir `/schedule`
3. Configurar:
   - **Nombre:** Briefing Diario de Búsqueda Laboral
   - **Cadencia:** Días de semana
   - **Hora:** 7:00 AM (personalizar según tu horario)
4. Pegar el prompt EXACTO de `tareas-cowork/daily-morning-briefing.md`
5. Guardar

## Opción 2: Ejecución Manual

En Claude Code:
```
Leer tareas-cowork/daily-morning-briefing.md y ejecutarlo
```

Ejecutar esto cada mañana hasta tener confianza en el output automatizado.

## Conectar Google Calendar

1. Abrir la app Claude Desktop
2. Ir a Configuración > Conectores
3. Hacer clic en 'Google Calendar'
4. Aparecerá una ventana de inicio de sesión de Google. Iniciar sesión con la cuenta de Google que tiene tu calendario de entrevistas.
5. Hacer clic en 'Permitir' para otorgar acceso
6. Deberías ver un check verde confirmando la conexión

Esto permite que el briefing verifique las entrevistas programadas e incluya recordatorios de prep en tu output diario.

## Qué Verificar en el Output

Después de las primeras ejecuciones, verificar:

- **Relevancia de roles:** ¿Los roles top coinciden realmente con tu plan de carrera?
- **Scores de fit:** ¿Los puntajes 1-100 se sienten correctos? Un rol que saltearías debe estar por debajo de 60.
- **Precisión del CV:** Cada bullet debe provenir de tu biblioteca de experiencias. Cero fabricación.
- **Solicitudes de conexión:** ¿Están personalizadas? ¿Aceptarías una si te la enviaran?
- **Coaching del pipeline:** ¿El consejo coincide con tu situación real?

## Solución de Problemas

- **Briefing no ejecuta:** La computadora debe estar encendida y Claude Desktop abierto a la hora programada
- **Roles irrelevantes:** Refinar el plan de carrera y la lista de empresas objetivo
- **CVs genéricos:** Tu biblioteca de experiencias está demasiado delgada. Agregar más detalle.
- **Solicitudes de conexión aburridas:** Agregar más detalle a tu biblioteca de experiencias (escuelas compartidas, empresas anteriores, ubicaciones)

## Ajustar con el Tiempo

El briefing mejora a medida que crece tu biblioteca de contexto. Después de cada semana:
- Actualizar `rastreador-conexiones.md` con nuevas conexiones
- Actualizar `rastrear-postulaciones` con estados de postulaciones
- Revisar y ajustar `empresas-objetivo.md` basándote en qué está funcionando
