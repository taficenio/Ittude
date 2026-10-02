# Parte 2: Networking - Viernes, 2 de Octubre de 2026

## Modo detectado (desde `plan-carrera.md`)

- **MODO REMOTO: activo.** "Remoto excluyente" es un filtro duro declarado el 2026-08-12. Se prioriza por empresas remote-friendly confirmadas y se agrega sugerencia de comunidad virtual (ver abajo).
- **MODO DIRECTOR+/EMPLEADO: no aplica.** El plan de carrera no indica nivel Director+ como objetivo único (está abierto entre IC Senior, Lead/Head, o especialización en IA), y el usuario no está actualmente empleado (contrato en Amplifire terminó hace ~1 mes, per `biblioteca-experiencias.md`).
- **MODO RETURNER: no aplica en sentido estricto.** El gap de empleo actual es de ~1 mes (transición normal entre roles, según el propio análisis en `plan-carrera.md`), no un gap extendido de carrera. No se activa el template de "reactivación de red" por gap -- pero igual aplica en espíritu: los 6 contactos prioritarios de referido están todos dormidos desde hace 8 a 16 años (ver sección de referidos abajo), así que los mensajes de esta corrida están redactados como reconexión cálida, no como pedido directo en frío.

---

## Solicitudes de Conexión (0 generadas -- bloqueo documentado, no falta de gaps)

**Gaps de cobertura reales y confirmados** (empresas de `empresas-objetivo.md` con menos de 4 conexiones en `rastreador-conexiones.md`): 99 de 108 empresas objetivo tienen cero conexiones de 1er grado, y de las 9 que sí tienen cobertura, Amazon (3), Apple (2), Google (2), Salesforce (2) y Atlassian (1) también califican como gap (<4). Solo Globant (16), Mercado Libre (16) y Microsoft (5) están por encima del umbral.

**Por qué no se generaron las 25 solicitudes por defecto:** generar una solicitud de conexión personalizada requiere identificar a una persona real específica (nombre, rol, punto de conexión verificable) en cada empresa con gap. Esta corrida automatizada no tiene acceso a búsqueda de personas de LinkedIn (sin browser ni API de LinkedIn disponible en este entorno cloud). Inventar 25 nombres de personas para completar la cuota por defecto sería fabricar identidades -- la misma disciplina anti-fabricación de `CLAUDE.md` ("NUNCA inventes... experiencia") aplica acá a personas, no solo a habilidades o proyectos: no hay forma de verificar que esas 25 personas existan o trabajen donde se diría que trabajan.

**Esto es un problema de acceso del entorno, no de falta de empresas objetivo con gap** (hay 99+ candidatas reales esperando).

**Recomendación concreta para destrabar esto:**
1. Exportar un `Connections.csv` actualizado de LinkedIn (o hacer búsquedas manuales de "[Empresa] Product Manager" / "[Empresa] recruiter") y correr `/solicitud-conexion [lote]` de forma interactiva -- ese skill sí puede generar los 25 mensajes personalizados una vez que vos (o una sesión con browser) identifiquen personas reales.
2. Alternativa sin esperar: usar LinkedIn "People also viewed" o "Ver conexiones de 2do grado" desde los 6 contactos de 1er grado ya mapeados abajo -- son el camino más rápido a nombres reales en empresas con gap.

---

## Seguimientos (Recién Conectados)

Ninguno. El sistema nunca envió una solicitud de conexión real todavía (0 solicitudes marcadas como enviadas en 53 días, confirmado en `briefings/2026-10-02-part1-roles.md`), así que no hay conexiones nuevas aceptadas en las últimas 48 horas para hacer seguimiento.

---

## Pedidos de Referido y Recordatorios

### Nuevos Pedidos de Referido

Estos 6 contactos son los de mayor prioridad en `rastreador-conexiones.md` -- conexiones reales de 1er grado, dormidas desde hace entre 8 y 16 años, en empresas Tier 1 sin ningún referido activado todavía. Es la acción de mayor apalancamiento del sistema hoy (ver Parte 1).

- **Elena Yndurain** -- Director AI Product Management, Microsoft (conectados desde 03 Jul 2021):
"Hola Elena, hace un tiempo que no hablamos pero tu rol como Directora de AI Product Management en Microsoft llamó mucho mi atención. Soy Product Leader con 15+ años de experiencia y acabo de terminar una Maestría en IA en la Universidad de Auckland. Estoy explorando roles de Product/AI Product y me encantaría una charla breve de 15 minutos para conocer tu perspectiva sobre cómo se ve el área hoy en Microsoft, y si hay espacio para una conversación de referido más adelante. ¿Te vendría bien?"

- **Virginia Silvero** -- Regional Recruiter Lead, South of LatAm, Globant (conectados desde 28 Oct 2010):
"Hola Virginia, ¡tanto tiempo! Nos conectamos hace años en Globant. Soy Product Leader con 15+ años de experiencia (fintech, healthtech, telecom) y acabo de terminar una Maestría en IA en la Universidad de Auckland. Estoy evaluando volver a sumarme a Globant en un rol de Product, y como Regional Recruiter Lead pensé que podrías orientarme sobre el proceso o, si ves fit, ayudarme con un referido. ¿Tenés 15 minutos para charlar esta semana?"

- **Melina Ruggeri** -- LATAM Recruiting Senior Manager, Salesforce (conectados desde 29 Abr 2017):
"Hola Melina, ¡hace mucho que no hablamos! Nos conectamos en 2017. Soy Product Leader con 15+ años de experiencia y especialización reciente en IA (Maestría en la Universidad de Auckland). Estoy mirando oportunidades de Product en Salesforce y, como Recruiting Senior Manager LATAM, me encantaría tu visión sobre el equipo de producto y, si corresponde, un referido. ¿Podemos coordinar una llamada corta?"

- **Pedro Alejandro Santamarina** -- Sr. Product Development Manager, Mercado Libre (conectados desde 12 Jul 2013):
"Hola Pedro, hace tiempo que no hablamos -- nos conectamos en 2013. Soy Product Leader con 15+ años de experiencia (fintech, healthtech, telecom) y recién terminé una Maestría en IA. Como Sr. Product Development Manager en Mercado Libre, sos el contacto de Product más senior que tengo en mi red hoy. Me encantaría 15 minutos para escuchar tu mirada sobre el equipo y, si ves fit, pedirte un referido."

- **Bernardo Manzella** -- Head of People & Capacity Strategy (AI Studios), Globant (conectados desde 28 Oct 2010):
"Hola Bernardo, ¡tanto tiempo! Nos conectamos en 2010. Vi que lideras People & Capacity Strategy para AI Studios en Globant -- justo el cruce entre IA y talento que me interesa, ya que acabo de terminar una Maestría en IA (Universidad de Auckland) sumada a mis 15+ años en Product. Me encantaría una charla breve para entender cómo está creciendo AI Studios y si hay espacio para una conversación de referido."

- **Maria Jose Trejo Conde** -- Regional Talent Acquisition IT Senior Analyst, Mercado Libre (conectados desde 22 Mar 2017):
"Hola María José, ha pasado tiempo desde que nos conectamos en 2017. Soy Product Leader con 15+ años de experiencia y acabo de completar una Maestría en IA. Vi tu rol en Talent Acquisition IT regional en Mercado Libre y me encantaría charlar 15 minutos sobre cómo se ve el área de Producto hoy, y si hay lugar para una conversación de referido más adelante. ¿Tenés disponibilidad esta semana?"

### Recordatorios (5+ días, sin respuesta)

Ninguno. Ningún pedido de referido fue enviado todavía (0 en 53 días) -- estos 6 son los primeros que el sistema redacta. Una vez que se marquen como enviados en `rastreador-conexiones.md`, esta sección empezará a poblarse a partir de 5 días sin respuesta.

### Networking virtual de esta semana (MODO REMOTO)

Unirte a **Product School Slack** o a la comunidad de **Lenny** (Lenny's Newsletter community) y comentar en 2-3 threads relevantes sobre Product/AI -- ambas tienen actividad regular de hiring managers y recruiters de empresas remote-first (GitLab, Deel, Automattic) que son Tier 1/2 en `empresas-objetivo.md`.

---

## Resumen y próxima acción

El cuello de botella no cambió respecto a Parte 1: 0 solicitudes de conexión y 0 referidos enviados en 53 días. Esta corrida no pudo generar las 25 solicitudes de conexión nuevas por falta de acceso a búsqueda de personas (ver sección de arriba), pero sí dejó redactados y listos para enviar los 6 pedidos de referido a contactos reales ya confirmados -- la acción de mayor apalancamiento disponible hoy sin depender de ninguna herramienta externa. Marcar en `rastreador-conexiones.md` cuáles se envían.
