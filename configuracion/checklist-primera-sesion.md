# Checklist de Primera Sesión

Trabajar en este orden. ~45 minutos en total para el setup, luego estás operativo.

## Setup

- [ ] Claude Code instalado (`claude --version` funciona)
- [ ] Carpeta del proyecto abierta en Cursor (layout de tres paneles)
- [ ] Claude Code iniciado en la terminal (`claude`)
- [ ] CLAUDE.md leído y resumido

## Biblioteca de Contexto (La Base)

- [ ] `biblioteca-experiencias.md` completado
  - Texto del CV pegado
  - Perfil de LinkedIn pegado
  - Claude combinó y organizó por categoría
  - Preguntas de seguimiento respondidas (proyectos no en CV/LinkedIn)
  - Banco de historias iniciado (apuntar a 10-15 historias STAR)
- [ ] `qa-master.md` completado
  - Estrategia y scripts de compensación
  - Preguntas comunes respondidas
  - Logística (autorización de trabajo, disponibilidad, fecha de inicio)
- [ ] `plan-carrera.md` completado
  - Nivel/industria/función rankeados
  - Análisis de direccionamiento de debilidades completo (2-3 debilidades con estrategias)
  - Oferta ideal definida
  - Mercado objetivo definido (LATAM / remoto global / ambos)

### Personas en Transición de Carrera

Si estás haciendo transición a PM desde otra función (ingeniería, consultoría, diseño, etc.):
- Al construir tu biblioteca de experiencias, decirle a Claude tu función actual y que estás pivotando a PM. Automáticamente mapeará tu experiencia a habilidades equivalentes de PM.
- En plan-carrera.md, setear Debilidad 1 como 'Sin título PM' -- Claude construye una estrategia de direccionamiento de debilidades específicamente para transiciones de carrera.
- Los skills de adaptar-cv, preparar-entrevista y trabajo-muestra tienen modos para personas en transición que se activan cuando tu biblioteca de experiencias no tiene títulos de PM.
- Tu experiencia ES relevante. Consultoría = gestión de stakeholders, pensamiento estratégico, análisis de datos. Ingeniería = profundidad técnica, empatía con usuarios, pensamiento sistémico. Diseño = research de usuarios, prototipado, iteración.

### Roles No-PM (SWE, Diseño, Data Science, Marketing, CS)

El sistema auto-detecta tu función objetivo desde plan-carrera.md. Al completar la biblioteca de contexto:
- **Biblioteca de experiencias:** Organizar por las categorías de habilidad de TU función, no por las de PM. Claude adapta las categorías cuando procesa tu CV.
- **Plan de carrera:** Setear tu Función/Tipo de Rol claramente (ej: "Staff Software Engineer" o "Head of Design"). Esto dispara comportamiento específico de función en los 18 skills.
- **Banco de historias:** Tus historias deben demostrar las competencias centrales de TU función. SWE: decisiones técnicas, diseño de sistemas, debugging. Diseño: crítica de diseño, defensa del usuario, alineación de stakeholders. DS: diseño de experimentos, decisiones de modelos, traducción al negocio.
- **Empresas objetivo:** `/investigar-empresa` funciona para cualquier rol. Los perfiles de empresas en datos-insider/ están orientados a PM, pero `/investigar-empresa` genera intel específico de función desde la web.

Los 18 skills se adaptan:
- `/adaptar-cv` genera CVs apropiados para la función (no CVs de PM)
- `/simular-entrevista` usa tipos de pregunta específicos de función (system design para SWE, revisión de portfolio para Diseño, caso de estudio para DS)
- `/negociar` usa datos de compensación y estrategias de negociación específicas de función
- `/retro-semanal` usa benchmarks específicos de función

## Targeting

- [ ] `empresas-objetivo.md` generado (~100 empresas)
- [ ] Lista revisada y reordenada por prioridad
- [ ] Top 10 empresas verificadas por exactitud

## Infraestructura

**Nota:** Cowork y Granola son mejoras opcionales. El sistema funciona completamente sin ellos — solo ejecutar skills manualmente en Claude Code.

- [ ] Briefing matutino configurado en Cowork (ver `morning-briefing-setup.md`)
- [ ] Google Calendar conectado (opcional)
- [ ] Granola instalado y carpeta de transcripciones configurada (opcional)

## Verificación

- [ ] Primera ejecución manual del briefing
- [ ] Output revisado: roles relevantes, CVs precisos, sin fabricación
- [ ] Archivos de contexto ajustados si el output estuvo mal
- [ ] Segunda ejecución confirma mejoras

## Estás Listo

Después de este checklist, tu rutina diaria es de 20-30 minutos:
1. Revisar el briefing matutino
2. Verificar los mejores CVs (3 min cada uno)
3. Enviar postulaciones
4. Enviar solicitudes de conexión y seguimientos
5. Construir trabajo muestra para la empresa de mayor prioridad (opcional, 30-45 min)
