# Templates de Trabajo Muestra

Tres templates para tres situaciones diferentes. Cada uno produce un documento de 1-2 páginas que demuestra que ya pensás como alguien de su equipo. El skill `/trabajo-muestra` usa estos como estructura base.

---

## Cómo Elegir Tu Tipo

| Situación | Tipo | Objetivo |
|---|---|---|
| Encontraste un rol y querés destacarte antes de postular | **para-conseguir-entrevista** | Ganar la entrevista mostrando insight único |
| Ya estás en el proceso y querés impresionar | **en-proceso** | Probar que podés hacer el trabajo haciéndolo |
| Arruinaste una pregunta específica de entrevista | **entrevista-específica** | Recuperarse mostrando tu proceso real |

---

## Template 1: Para Conseguir la Entrevista (Pre-Postulación / Outreach en Frío)

**Propósito:** Adjunto a tu postulación o enviado directamente al hiring manager. Gana la entrevista probando que entendés su producto y tenés una perspectiva diferenciada.

**Largo:** 1 página. Máx 2.

**Research requerido antes de escribir (los hooks):**
- [ ] Llamada de earnings o anuncio de funding más reciente (prioridades del CEO)
- [ ] Reseñas de productos: App Store, Play Store, G2, TrustRadius (quejas reales de usuarios)
- [ ] Posts recientes de blog de producto/ingeniería (qué están construyendo públicamente)
- [ ] Quejas públicas de usuarios: Twitter/X, Reddit, Hacker News (puntos de dolor conocidos)
- [ ] Lanzamientos o cambios recientes de features (señales de dirección del producto)

Extraer 3-5 hooks específicos de este research. Estos hacen el documento imposible de descartar como genérico.

### Estructura

```markdown
# [Título Específico, ej: "Reducir el Abandono en el Flujo de Checkout de Mercado Pago"]
[Tu Nombre] | [Fecha] | Para: [Título del Rol] en [Empresa]

## Por Qué Escucharme
[2-3 oraciones conectando TU experiencia específica con SU problema específico.
Sacar directamente de biblioteca-experiencias.md. No "Soy PM con 8 años de experiencia"
sino "En [Empresa], reduje el abandono de checkout en un 34% en un flujo de pagos
manejando $2B anualmente -- un problema estructuralmente similar a lo que veo en
la experiencia de billing de [Empresa Objetivo]."]

## La Observación
[1-2 párrafos. Empezar con una observación específica y basada en datos sobre su producto.
Referenciar una queja real de usuario, una métrica pública o algo que notaste usando
el producto vos mismo. Esto prueba que hiciste el trabajo.]

[Ejemplo de hook: "En el earnings del Q3, [CEO] mencionó la conversión en checkout como una
iniciativa clave. Mirando 127 reseñas recientes en la App Store que mencionan 'checkout,'
emergen tres patrones..."]

## Análisis
[Desglosar el problema. 3-5 puntos específicos. Cada uno fundamentado en datos u
observaciones, no en teoría. Mostrar el pensamiento de producto, no un framework.]

1. **[Punto específico]:** [Evidencia de hooks de research + tu interpretación]
2. **[Punto específico]:** [Evidencia + interpretación]
3. **[Punto específico]:** [Evidencia + interpretación]

## Recomendaciones
[2-3 recomendaciones específicas y accionables. Cada una debe ser:]
- No obvia (no "mejorar el onboarding")
- Fundamentada en tus hooks de research
- Conectada a tu experiencia única
- Reconociendo trade-offs (cada recomendación tiene un costo)

### 1. [Título de Recomendación]
[Qué hacer, por qué funciona, qué trade-off aceptar, qué métrica monitorear]

### 2. [Título de Recomendación]
[Misma estructura]

### 3. [Título de Recomendación]
[Misma estructura]

## Qué Me Gustaría Explorar Juntos
[1-2 oraciones enmarcando la próxima conversación. Señalar que sabés que te
falta contexto interno y querés aprender, no solo presentar una pitch.]
```

---

## Template 2: En Proceso (Durante los Loops de Entrevista)

**Propósito:** Enviado entre rondas o como tarea para llevar a casa. Prueba que podés hacer el trabajo real del rol. Este es un mini-PRD o propuesta de producto con alcance ajustado al charter del hiring manager.

**Largo:** 1-2 páginas. Denso. Sin relleno.

**Research requerido antes de escribir:**
- [ ] Todo del research de "para-conseguir-entrevista", MÁS:
- [ ] El LinkedIn del HM (¿de qué es responsable?)
- [ ] Cambios recientes de producto en el área del HM específicamente
- [ ] Landscape competitivo para esta área de producto específica
- [ ] Señales internas de tus entrevistas (¿qué problemas mencionaron los entrevistadores?)

### Estructura

```markdown
# [Título de Propuesta, ej: "Propuesta de Feature: Recordatorios Inteligentes de Facturas para Facturación de Stripe"]
[Tu Nombre] | [Fecha] | Para: [Título del Rol] en [Empresa]

## Por Qué Escucharme
[Mismo formato que para-conseguir-entrevista. 2-3 oraciones conectando tu experiencia
con esta propuesta específica. Ser preciso sobre el paralelo.]

## Definición del Problema
[Definir el problema desde la perspectiva del USUARIO, no de la empresa. Incluir:]
- Quién tiene este problema (segmento específico de usuario)
- Qué tan doloroso es (datos: tickets de soporte, reseñas, correlación con churn)
- Por qué importa ahora (presión de mercado, amenaza competitiva, prioridad del CEO)

## Estado Actual
[Qué hace el producto hoy. Ser lo suficientemente específico para que el HM sepa que
realmente usaste el producto. Bienvenidas las descripciones de screenshots o flujos.]

## Solución Propuesta

### User Stories
- Como [tipo de usuario], quiero [acción] para que [resultado]
- Como [tipo de usuario], quiero [acción] para que [resultado]
- Como [tipo de usuario], quiero [acción] para que [resultado]

### Flujos Clave
[Describir los 2-3 flujos de usuario más importantes. Si construiste un prototipo
usando el template de prototipo, referenciarlo o linkearlo aquí.]

1. **[Nombre del flujo]:** [Descripción paso a paso]
2. **[Nombre del flujo]:** [Descripción paso a paso]

### Qué NO Estoy Proponiendo (Límites de Alcance)
[Declarar explícitamente qué está fuera de alcance y por qué. Esto demuestra
priorización y evita que el HM piense que sos ingenuo sobre la complejidad.]

## Contexto Competitivo
[Qué hacen los competidores aquí. No una matriz de features -- un insight sobre
diferentes elecciones estratégicas y sus trade-offs.]

## Métricas de Éxito
- **Principal:** [métrica + objetivo, ej: "Reducir pagos tardíos en un 20% en 6 meses"]
- **Secundaria:** [métrica + objetivo]
- **Guardarraíl:** [métrica que NO debe empeorar, ej: "Volumen de tickets de soporte se mantiene estable"]

## Enfoque por Fases
| Fase | Alcance | Estimación de Timeline | Riesgo Principal |
|---|---|---|---|
| 1 (MVP) | [versión mínima viable] | [semanas] | [riesgo más grande] |
| 2 | [iteración basada en datos de Fase 1] | [semanas] | [riesgo] |
| 3 | [visión completa] | [semanas] | [riesgo] |

## Preguntas Abiertas
[3-5 preguntas que necesitarías datos internos para responder. Muestra
honestidad intelectual y prepara la próxima conversación.]
```

---

## Template 3: Entrevista Específica (Recuperación Post-Entrevista)

**Propósito:** Enviado como adjunto de seguimiento cuando arruinaste una pregunta específica en una entrevista. Prueba que tu proceso real es más fuerte que tu respuesta improvisada.

**Largo:** 1 página.

**Cuándo usar:**
- Saltaste a una solución sin explorar el problema
- Te bloqueaste con métricas o estructura
- Diste una respuesta superficial a una pregunta profunda
- El entrevistador profundizó en un área donde tu respuesta fue débil

### Estructura

```markdown
# [Título, ej: "Cómo Realmente Abordaría: Priorizar el Roadmap de Features SMB de Stripe"]
[Tu Nombre] | [Fecha] | Seguimiento de la entrevista con [Ronda/Nombre del Entrevistador]

## Contexto
[1-2 oraciones. Nombrar la pregunta. Reconocer que tu respuesta en vivo estuvo incompleta.]

[Ejemplo: "En nuestra conversación, me preguntaste cómo priorizaría el roadmap de
features SMB. Salté a una respuesta de framework. Así se ve mi proceso real cuando
tengo tiempo para hacerlo bien."]

## Mi Proceso

### Paso 1: Definir la Decisión
[¿Exactamente qué estamos decidiendo? Enmarcar la pregunta de priorización con precisión.
Mostrar que empezás aclarando el scope, no saltando a soluciones.]

### Paso 2: Reunir Señales
[¿Dónde buscaría datos? Ser específico para esta empresa:]
- **Datos de uso:** [qué consultaría y por qué]
- **Research de usuarios:** [qué preguntas haría a qué segmentos]
- **Análisis competitivo:** [qué miraría y qué aprendería]
- **Input de stakeholders:** [con quién hablaría y qué preguntaría]
- **Restricciones del negocio:** [qué necesitaría entender sobre el modelo de negocio]

### Paso 3: Sintetizar
[Cómo combinaría estos inputs en un framework de decisión. No un RICE genérico --
un framework específico para este problema que pese las dimensiones que realmente importan aquí.]

### Paso 4: La Recomendación
[Dado lo que sé públicamente, aquí está mi mejor hipótesis sobre cómo priorizaría.
Incluir features/iniciativas específicas con razonamiento.
Reconocer qué cambiaría con datos internos.]

## Por Qué Escucharme
[Conectar con una experiencia paralela donde corriste exactamente este proceso.
Sacar de la biblioteca de experiencias. Incluir el outcome específico.]

## Qué Exploraría a Continuación
[Enmarcar la conversación que tendrías con el HM.
2-3 preguntas específicas que demuestran tu profundidad.]
```

---

## Checklist de Calidad (Todos los Tipos)

Antes de enviar cualquier trabajo muestra, verificar:

- [ ] **Hooks específicos de empresa:** Al menos 3 referencias a datos específicos y recientes de la empresa (earnings, reseñas, lanzamientos)
- [ ] **"Por Qué Escucharme" está fundamentado:** Cada claim rastrea hacia biblioteca-experiencias.md
- [ ] **Sin oraciones genéricas:** Leer cada oración y preguntarse "¿Podría esto aplicar a cualquier empresa?" Si sí, reescribir.
- [ ] **Sin lenguaje que suena a IA:** Sin "sinergias," "landscape," "aprovechar," "robusto," "optimizar," "de vanguardia"
- [ ] **Trade-offs reconocidos:** Cada recomendación tiene un costo o riesgo mencionado
- [ ] **Menos de 2 páginas:** Más corto siempre es mejor. Si podés cortar un párrafo sin perder el argumento, cortarlo.
- [ ] **Métricas reales:** Al menos 2-3 puntos de datos de fuentes públicas
- [ ] **Accionable:** Un PM en su equipo podría llevar esto a una reunión de planning
- [ ] **Prototipo incluido (opcional):** Si usaste prototype-prompt-template.md, linkearlo

## Después de Escribir

1. Ejecutar `/revisar-como-hiring-manager` para obtener el puntaje desde la perspectiva del HM
2. Abordar todos los flags de "contenido genérico" y "contenido que suena a IA"
3. Objetivo de puntaje: Especificidad 8+, Product Sense 7+, Insight Único 7+, Accionabilidad 7+
4. Si la respuesta al test de reunión es "No" o "Tal vez", revisar antes de enviar
