# Tracker de Referidos

Rastrear el progreso de referidos para cada rol que estés persiguiendo activamente. Un referido es 5 veces más efectivo que una postulación en frío. Este tracker asegura que ningún pedido de referido caiga en el olvido.

**Cómo usar:**
- Crear una sección por rol activo
- Actualizar después de cada interacción relacionada con referidos
- El briefing matutino verifica este archivo diariamente y marca los pedidos sin respuesta
- `/pedir-referido` auto-genera los mensajes; vos rastreás el progreso aquí

**Definiciones de estado del referido:**
- **Sin empezar:** Todavía no identifiqué una conexión
- **Conexión identificada:** Encontré a alguien en la empresa pero no lo pedí aún
- **Pedido enviado:** Envié el pedido de referido; esperando respuesta
- **Acordado:** Dijeron que sí; el referido aún no fue enviado
- **Enviado (solo ATS):** Lo enviaron a través del portal de referidos del ATS
- **Referido fuerte (HM contactado):** Le enviaron un mensaje directo al hiring manager por Slack/email -- este es el estándar de oro
- **Rechazado:** Dijeron que no (notar por qué; ajustar enfoque para la próxima persona)
- **Sin respuesta:** Envié el pedido hace 5+ días sin respuesta (el briefing matutino marca estos)

---

## [Nombre de Empresa] - [Título del Rol]

**Estado de postulación:** [Sin postular aún / Postulé el FECHA / Etapa de entrevista]
**URL de la oferta:** [link]
**Hiring manager:** [Nombre, si se conoce] | [URL de LinkedIn]

### Intento de Referido 1

| Campo | Detalles |
|---|---|
| **Nombre del contacto** | [Nombre] |
| **Su rol** | [Título en la empresa] |
| **Solidez de la relación** | [Cercano / Nos conocimos una vez / Solo LinkedIn / Amigo de amigo] |
| **Cómo están conectados** | [Cómo lo conocés: escuela, ex-colega, LinkedIn en frío, intro de X] |
| **Pedido enviado** | [Fecha] vía [Mensaje LinkedIn / Email / Mensaje de texto / En persona] |
| **Respuesta** | [Fecha] - [Acordó / Rechazó / Sin respuesta aún] |
| **Tipo de referido** | [Envío ATS / Ping HM / Ambos] |
| **¿Compartió nombre del HM?** | [Sí - Nombre: ___ / No / No pregunté] |
| **Seguimiento enviado** | [Fecha del mensaje de push de referido fuerte, si aplica] |
| **Estado** | [Sin empezar / Pedido enviado / Acordado / Enviado / Referido fuerte / Rechazado / Sin respuesta] |
| **Notas** | [Cualquier contexto: "Dijo que lo haría después de sus vacaciones" / "Sugirió que también hable con [Nombre]"] |

### Intento de Referido 2 (si el primero no funcionó)

| Campo | Detalles |
|---|---|
| **Nombre del contacto** | [Nombre] |
| **Su rol** | [Título] |
| **Solidez de la relación** | [Cercano / Nos conocimos una vez / Solo LinkedIn / Amigo de amigo] |
| **Cómo están conectados** | [Cómo lo conocés] |
| **Pedido enviado** | [Fecha] vía [canal] |
| **Respuesta** | [Fecha] - [resultado] |
| **Tipo de referido** | [ATS / Ping HM / Ambos] |
| **¿Compartió nombre del HM?** | [Sí/No] |
| **Seguimiento enviado** | [Fecha] |
| **Estado** | [estado] |
| **Notas** | [contexto] |

### Resultado del Referido

| Métrica | Valor |
|---|---|
| **Personas pedidas** | [N] |
| **Personas que acordaron** | [N] |
| **Referidos ATS enviados** | [N] |
| **Pings de HM confirmados** | [N] |
| **Tiempo desde primer pedido hasta referido** | [N días] |
| **Impacto en la postulación** | [Conseguí entrevista / Sin impacto claro / Desconocido] |

---

## [Nombre de Empresa] - [Título del Rol]

**Estado de postulación:** [estado]
**URL de la oferta:** [link]
**Hiring manager:** [Nombre] | [URL de LinkedIn]

### Intento de Referido 1

| Campo | Detalles |
|---|---|
| **Nombre del contacto** | |
| **Su rol** | |
| **Solidez de la relación** | |
| **Cómo están conectados** | |
| **Pedido enviado** | |
| **Respuesta** | |
| **Tipo de referido** | |
| **¿Compartió nombre del HM?** | |
| **Seguimiento enviado** | |
| **Estado** | |
| **Notas** | |

### Resultado del Referido

| Métrica | Valor |
|---|---|
| **Personas pedidas** | |
| **Personas que acordaron** | |
| **Referidos ATS enviados** | |
| **Pings de HM confirmados** | |
| **Tiempo desde primer pedido hasta referido** | |
| **Impacto en la postulación** | |

---

<!-- Copiar la sección de arriba para cada nuevo rol que estés persiguiendo. -->

## Dashboard Resumen

Actualizar semanalmente (o dejar que `/retro-semanal` lo calcule):

| Métrica | Esta Semana | Total | Objetivo |
|---|---|---|---|
| Roles activos siendo perseguidos | | | 5-10 |
| Pedidos de referido enviados | | | 1 por postulación |
| Referidos recibidos | | | 60%+ de postulaciones |
| Referidos fuertes (HM contactado) | | | 30%+ de referidos |
| Días promedio desde pedido hasta referido | | | Menos de 5 días |
| Postulaciones con referidos | | | 60%+ del total |
| Tasa de respuesta (con referido) | | | 15-25% |
| Tasa de respuesta (sin referido) | | | 3-5% |

## Playbook de Pedido de Referido (Referencia Rápida)

**Mensaje 1 - Pedido Inicial:**
Generado por `/pedir-referido`. Enviar dentro de las 24 horas de postular o antes de postular.

**Mensaje 2 - Push de Referido Fuerte (después de que acuerden):**
"¡Muchas gracias! Un pedido más -- ¿podrías también escribirle directamente al hiring manager ([Nombre] si lo tenés) por LinkedIn o email? Un referido por ATS está perfecto, pero un mensaje directo tuyo hace que sea 5 veces más probable que reciba atención."

**Mensaje 3 - Recordatorio Sin Respuesta (5+ días después del pedido inicial):**
Mantenerlo corto y sin presión. Un recordatorio. Si no hay respuesta después del recordatorio, pasar a otro contacto.

**Cuando rechazan:**
- Agradecerles genuinamente
- Preguntar: "¿Hay alguien más en el equipo a quien sugerirías que contacte?"
- Notar el motivo en el tracker (muy nuevo, no conoce al HM, política de empresa) -- ayuda a calibrar pedidos futuros

**Cuando acuerdan pero no siguen (7+ días):**
- Un recordatorio amable: "Hola [Nombre], solo chequeando si pudiste enviar el referido. Sin problema si el timing no funciona."
- Si aún nada después del recordatorio, pasar a otro contacto. No enviar un tercer mensaje.
