# Template de Prompt para Prototipo

Después de completar tu trabajo muestra de 1-pager, usar este prompt para generar un prototipo clickeable de tu recomendación clave. Un prototipo funcionando convierte tu análisis escrito en algo sobre lo que el hiring manager puede hacer clic -- demuestra capacidad de ejecución, no solo pensamiento estratégico.

**Presupuesto de tiempo:** ~30 minutos de iteración. No sobre-invertir. El prototipo apoya el 1-pager; no es el entregable principal.

**Herramientas:** Pegar el prompt de abajo en cualquiera de estas:
- **Claude Code** (mejor para interacciones complejas, mockups de API)
- **Lovable** (mejor para UI pulida, iteración rápida)
- **v0 by Vercel** (mejor para prototipos a nivel de componentes)
- **Bolt** (bueno para mockups full-stack)
- **Replit** (bueno para prototipos con muchos datos)

---

## El Prompt

Copiar todo entre los marcadores `---`. Completar las secciones entre corchetes.

---

Construir un prototipo clickeable para el área de producto [Nombre del Producto] de [Nombre de Empresa].

Contexto: Estoy entrevistando para [título del rol] en [Nombre de Empresa] y creé un análisis de producto con estas recomendaciones:
1. [Recomendación 1 - la que hay que prototipar. Ser específico: ¿qué hace, para quién es, qué problema resuelve?]
2. [Recomendación 2 - descripción breve]
3. [Recomendación 3 - descripción breve]

Construir un prototipo interactivo de la recomendación #1.

**Flujo de usuario:**
- [Paso 1: Qué ve el usuario primero, ej: "Dashboard mostrando estado de facturas con un nuevo panel de 'Recordatorios Inteligentes'"]
- [Paso 2: Qué hace clic el usuario/qué hace, ej: "El usuario hace clic en 'Configurar Recordatorios' y ve un asistente de configuración"]
- [Paso 3: La interacción clave, ej: "El usuario configura reglas de recordatorio basadas en antigüedad y monto de la factura, ve preview del email de recordatorio"]
- [Paso 4: El resultado, ej: "Pantalla de confirmación mostrando impacto proyectado: '34% menos pagos tardíos basado en tu historial de facturas'"]

**Pantallas necesarias:**
1. [Nombre de pantalla 1 y qué muestra]
2. [Nombre de pantalla 2 y qué muestra]
3. [Nombre de pantalla 3 y qué muestra]

**Requisitos de diseño:**
- Coincidir con el lenguaje de diseño de [Nombre de Empresa]. Sus colores de marca son [colores si se conocen, o "buscar su sitio web"]. Su estilo de UI es [limpio/denso/juguetón/enterprise -- describir lo que ves en su producto].
- Usar su estilo tipográfico (serif/sans-serif, peso, espaciado)
- La navegación debe sentirse como si perteneciera dentro de su producto existente
- Incluir datos ficticios realistas que coincidan con su dominio (ej: nombres de empresas que suenan reales para un producto B2B, montos en pesos/dólares realistas para un producto fintech)

**Stack tecnológico:** Usar React y Tailwind CSS.

**Prioridad:** Verse real > estar completo. Esto es para una postulación de trabajo, no para producción. Enfocarse en:
1. El happy path principal funcionando end-to-end
2. Datos de aspecto realista y UI pulida
3. Una o dos micro-interacciones que se sientan premium (estados hover, transiciones)

NO construir:
- Flujos de autenticación o login
- Lógica de backend (mockear todos los datos)
- Edge cases o estados de error
- Responsividad móvil (solo desktop está bien)

---

## Después de Generar: Checklist de Iteración

Gastar el tiempo restante en esto, en orden:

1. **¿Se ve como si perteneciera a su producto?** Si no, ajustar colores, tipografía, espaciado.
2. **¿Funciona el flujo principal end-to-end?** Hacer clic en cada paso. Arreglar la navegación rota.
3. **¿Son realistas los datos ficticios?** Reemplazar "Lorem ipsum" y "Empresa A" con ejemplos apropiados para el dominio.
4. **Un pasaje de pulido:** Agregar un estado hover, una transición o una visualización de datos que lo haga sentir premium.
5. **Screenshot o deploy:** Tomar 2-3 screenshots para tu doc de trabajo muestra, o deployar en Vercel/Netlify para un link en vivo.

## Cómo Incluir en Tu Trabajo Muestra

**Opción A: Link en vivo (preferido)**
Deployar en Vercel o Netlify (gratis). Incluir la URL en tu trabajo muestra bajo recomendaciones:
"Prototipé esta recomendación: [link]. Demuestra el flujo central de usuario para [feature]."

**Opción B: Screenshots**
Tomar 2-3 screenshots de las pantallas clave. Incluirlos en tu doc de trabajo muestra con captions explicando el flujo.

**Opción C: Grabación de pantalla**
Grabar un recorrido de 30-60 segundos usando grabación de pantalla de Windows (Win+G) o Loom. Adjuntar el link del video.

## Errores Comunes a Evitar

- **Sobre-construir:** Necesitás 3-4 pantallas, no 15. Parar en el happy path.
- **Fidelidad incorrecta:** Esto debe verse como un producto real, no un wireframe. Usar colores, texto real, datos realistas.
- **Ignorar su lenguaje de diseño:** Un prototipo que no se parece nada a su producto socava el punto. Pasar 5 minutos en su sitio web primero.
- **Sin contexto en el prompt:** Cuanto más específico seas sobre el flujo de usuario, mejor será el output. Prompts vagos producen prototipos vagos.
- **Gastar más de 30 minutos:** Retornos decrecientes. Lanzarlo y seguir adelante.
