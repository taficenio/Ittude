# Template de CV Base

Este es tu CV maestro. Cada output de `/adaptar-cv` comienza desde esta base y selecciona/reescribe bullets para coincidir con una oferta específica. Mantener este archivo completo -- incluir todo. Adaptar es sobre seleccionar el subconjunto correcto, no escribir desde cero cada vez.

## Instrucciones

1. Pegá tu CV actual abajo, siguiendo la estructura
2. Ejecutar: "Ayudame a organizar mi CV base usando la biblioteca de experiencias"
3. Claude cruzará referencias con `biblioteca-contexto/biblioteca-experiencias.md` y completará la versión estructurada
4. Revisar, agregar lo que falte, eliminar lo que esté desactualizado
5. Este archivo debe tener MÁS bullets que cualquier CV adaptado individual (los CVs adaptados seleccionan los mejores 3-5 por rol)

---

## [TU NOMBRE COMPLETO]

**Contacto:**
[Email] | [Teléfono] | [URL de LinkedIn] | [Ciudad, País]

---

### Resumen

<!--
Escribir 2-3 versiones abajo. /adaptar-cv selecciona la mejor basándose en la oferta
y puede modificarla para incorporar la estrategia de direccionamiento de debilidades de plan-carrera.md.
Mantener cada una en menos de 3 líneas. Liderar con tu calificación más fuerte para el tipo de rol objetivo.
-->

**Versión A (para [tipo de rol, ej: "roles de Growth PM"]):**
[Resumen de 2-3 oraciones enfatizando experiencia de crecimiento/métricas. Incluir años de experiencia, métrica más grande de scope/impacto y la habilidad que más te diferencia.]

**Versión B (para [tipo de rol, ej: "roles de PM en IA/ML"]):**
[Resumen de 2-3 oraciones enfatizando experiencia técnica/IA. Reenmarcar tu experiencia hacia este dominio.]

**Versión C (para [tipo de rol, ej: "roles de PM de Plataforma"]):**
[Resumen de 2-3 oraciones enfatizando experiencia de plataforma/infraestructura.]

---

### Experiencia

<!--
Para cada rol, incluir TODOS los bullets que podrías usar alguna vez.
/adaptar-cv selecciona los mejores 3-5 por rol basándose en la oferta.
Etiquetar cada bullet con la categoría de habilidad que demuestra.
Usar este formato: métrica + contexto + acción + resultado.
Cada bullet debe tener un número. Si no lo tiene, agregarlo o marcarlo para la biblioteca de experiencias.
-->

#### [Título del Puesto] | [Nombre de Empresa] | [Fecha Inicio] - [Fecha Fin/Presente]
[Declaración de scope de una línea: tamaño de equipo, área de producto, base de usuarios, responsabilidad de ingresos]

- [CRECIMIENTO] [Bullet con métrica específica, ej: "Aumenté activación de usuarios del 23% al 38% (65% de aumento) rediseñando el flujo de onboarding, impactando 2M+ nuevos usuarios anualmente"]
- [CRECIMIENTO] [Otro bullet de crecimiento/métricas]
- [TÉCNICO] [Bullet demostrando profundidad técnica]
- [LIDERAZGO] [Bullet demostrando liderazgo cross-funcional, incluir tamaño del equipo]
- [ESTRATEGIA] [Bullet demostrando pensamiento estratégico]
- [EJECUCIÓN] [Bullet demostrando capacidad de lanzamiento/ejecución]
- [CLIENTE] [Bullet demostrando insight del cliente o research]

#### [Título Anterior] | [Nombre de Empresa] | [Fecha Inicio] - [Fecha Fin]
[Declaración de scope de una línea]

- [TAG] [Bullet]
- [TAG] [Bullet]
- [TAG] [Bullet]
- [TAG] [Bullet]
- [TAG] [Bullet]

#### [Título Anterior] | [Nombre de Empresa] | [Fecha Inicio] - [Fecha Fin]
[Declaración de scope de una línea]

- [TAG] [Bullet]
- [TAG] [Bullet]
- [TAG] [Bullet]

<!--
Agregar tantos roles como sean relevantes. Para roles más antiguos (5+ años atrás), mantener en 2-3 bullets.
Para tus 2 roles más recientes, incluir 5-8 bullets cada uno.
-->

---

### Habilidades

<!--
Organizar por categoría. /adaptar-cv reordena estas para coincidir con keywords de la oferta.
Incluir tanto el término completo como la abreviación para el matching de ATS.
Solo incluir habilidades sobre las que puedas hablar en una entrevista.
-->

**Product Management:** [ej: Roadmapping, Pruebas A/B (Experimentación), PRDs, User Stories, OKRs, Estrategia de Producto, Go-to-Market]

**Técnico:** [ej: SQL, Python, Análisis de Datos, Diseño de APIs, Machine Learning (ML), Agile/Scrum]

**Herramientas:** [ej: Amplitude, Mixpanel, Tableau, Figma, Jira, Notion, dbt]

**Dominio:** [ej: Fintech, Pagos, Productos de Consumo, B2B SaaS, Marketplace, eCommerce LATAM]

---

### Educación

#### [Título] | [Nombre de Universidad] | [Año de Egreso]
[Honores, materias relevantes o actividades -- solo si son notables o relevantes para el rol]

#### [Título] | [Nombre de Universidad] | [Año de Egreso]
[Igual que arriba]

---

### Certificaciones / Adicional (Opcional)

- [Certificación, ej: "AWS Cloud Practitioner"]
- [Logro notable, ej: "Speaker, ProductConf LATAM 2024"]
- [Publicación, ej: "Autor, ittude-agile.com (50K suscriptores)"]
- [Idiomas si son relevantes para el rol/ubicación]

---

## Referencia de Tags de Bullets

Usar estos tags al agregar nuevos bullets para que `/adaptar-cv` pueda hacerles match eficientemente con los requisitos de la oferta:

| Tag | Qué Demuestra | Cuando la Oferta Pide |
|---|---|---|
| CRECIMIENTO | Métricas de ingresos, engagement o adopción | "Drive growth," "mejorar métricas," "data-driven" |
| TÉCNICO | Colaboración con ingeniería, decisiones técnicas, APIs, ML | "PM técnico," "trabajar con ingenieros," "system design" |
| LIDERAZGO | Gestión de personas, trabajo cross-funcional, influencia | "Liderar equipo," "cross-funcional," "gestión de stakeholders" |
| ESTRATEGIA | Visión, roadmap, análisis competitivo, sizing de mercado | "Estrategia de producto," "visión de producto," "análisis de mercado" |
| EJECUCIÓN | Lanzar productos, gestión de proyectos, plazos | "Lanzar productos," "orientado a ejecución," "entregar resultados" |
| CLIENTE | Research de usuarios, entrevistas a clientes, decisiones basadas en insights | "Enfocado en cliente," "research de usuario," "voz del cliente" |
| DOMINIO | Conocimiento específico de industria | Industria específica mencionada en la oferta |

## Mantenimiento

- Actualizar este archivo cuando obtengas nuevas métricas o lances algo notable
- Después de cada corrida de `/adaptar-cv`, verificar si los bullets seleccionados son los más fuertes disponibles -- si no, mejorar la base
- Trimestral: eliminar bullets desactualizados, agregar logros recientes
- Cruzar referencias con `biblioteca-contexto/biblioteca-experiencias.md` para asegurarse de que no falte nada
