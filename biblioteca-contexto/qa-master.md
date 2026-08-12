# Documento Maestro de Q&A

## Instrucciones

Completá cada respuesta una vez. El OS las usa para formularios de postulación, entrevistas simuladas y paquetes de preparación. Claude te guiará por cada sección si ejecutás: `Ayudame a completar el doc de Q&A maestro`

## Compensación

### "¿Cuál es tu sueldo actual?"
**Estrategia:** Evitar compartir. Redirigir al rango del rol.
**Script:** [PENDIENTE — te propongo uno apenas confirmes tu rango objetivo abajo.]
**Rango de respaldo si insisten:** [PENDIENTE]
**Fuente de datos para el rango:** [PENDIENTE — se completa con `/investigar-salario` una vez que haya una oferta o industria concreta para anclar el research.]

### "¿Cuáles son tus expectativas de compensación?"
**Rango objetivo:** [PENDIENTE]
**Fuente:** [PENDIENTE — `/investigar-salario`]
**Script:** [PENDIENTE]

## Preguntas Comunes

### "¿Por qué estás dejando tu rol actual?"
**[ACTUALIZADO 2026-08-11 — la versión anterior tenía la fecha de fin mal, corregida acá]:** El contrato en Amplifire (2 años y medio, Ene 2024–Jul 2026) terminó el mes pasado tras completar la implementación del proyecto (el chatbot de soporte con IA, RAG y LLM). Hoy busco activamente un rol que permita una proyección de desarrollo profesional a largo plazo. [Nota: ya no hace falta mencionar proyectos freelance/data engineering para "llenar" un gap — el gap real es de solo ~1 mes, no necesita relleno narrativo.]

### "¿Por qué querés trabajar en [empresa]?"
[Se completa dinámicamente por `/preparar-entrevista` para cada empresa específica, usando `datos-insider/company-intel/` y `empresas-objetivo.md`.]

### "¿Cuál es tu mayor debilidad?"
**[Confirmado por el usuario]:** En UCG, no prioricé a tiempo una feature que daba acceso a mandos medios para autorizar órdenes de trabajo de los operarios. Esas posiciones intermedias eran justamente las que debían aprobar esas órdenes, y la falta de esa feature impactó directamente en una métrica de defectos. Después de esto, cambié mi forma de priorizar: empecé a usar frameworks específicos (WSJF, Kano Model) e involucrar activamente a stakeholders de distintas áreas antes de definir prioridades, en vez de decidir de forma más aislada.

### "¿Cuál es tu mayor fracaso?"
**[Confirmado por el usuario]:** En Accenture, durante la implementación de Siebel (CRM) para Telefónica, el foco estuvo puesto en la migración técnica y el relevamiento de requerimientos, sin un plan de gestión del cambio para acompañar a los usuarios finales. El sistema no logró adopción real por parte de los usuarios, que prefirieron seguir con el sistema viejo. Aprendí que una migración técnica exitosa no garantiza adopción: hoy planificaría con un equipo de gestión del cambio cómo capacitar a los usuarios no solo en el "cómo" sino en el "por qué" el nuevo sistema mejora su trabajo.

### "¿Dónde te ves en 3 años?"
**[Confirmado por el usuario — tres caminos posibles, a definir según cómo evolucione la búsqueda]:** Me veo en uno de tres caminos: (1) consolidado como Product Owner/Manager Senior como IC, (2) en un rol de liderazgo de equipo tipo Lead o Head of Product, o (3) especializándome en profundidad en IA. La dirección específica depende de qué oportunidad ofrezca la mejor proyección de desarrollo a largo plazo — el criterio ancla (ver `plan-carrera.md`) es la organización y su capacidad de darme crecimiento sostenido, más que un título específico.

### "Contame sobre vos" (máx 2 min)
[Se genera dinámicamente por `/preparar-entrevista` para cada empresa, usando el framework de direccionamiento de debilidades de `plan-carrera.md`. No lo redacto acá como texto fijo porque pierde precisión si no está adaptado a la oferta puntual.]

## Logística

### Modalidad de Trabajo / Preferencia
**[Completado desde `plan-carrera.md`]:** Remoto preferido. Abierto a roles remotos con empresas de Argentina, LatAm, USA, Canadá o Europa.

### Disponibilidad de Fecha de Inicio
Inmediata.

### "¿Estás entrevistando en otras empresas?"
Sí, actualmente en proceso con otras empresas.
**Script sugerido:** "Sí, estoy en conversaciones con algunas empresas en este momento, pero este rol es una prioridad para mí por [razón específica de la empresa — completar en `/preparar-entrevista`]."

### Disponibilidad para Viajes
No tiene disponibilidad para viajar, aunque lo considera potencialmente discutible según el rol/empresa. [Nota: matizar esto en conversación si el viaje es un requisito puntual y no frecuente, en vez de descartar la oferta de entrada.]

### Autorización de Trabajo
Ciudadano argentino, con autorización de trabajo en Argentina. Para roles en USA, Canadá o Europa, requeriría sponsorship de visa — no tiene autorización de trabajo propia en esos países. [Nota: esto es un filtro real para `/investigar-empresa` y `/evaluar-oferta` — priorizar roles remotos globales que acepten contratación desde Argentina/LatAm sin requerir relocalización, o empresas que ofrezcan sponsorship activamente.]
