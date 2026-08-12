> **¿Primera vez?** Leé [EMPEZAR-ACA.md](EMPEZAR-ACA.md) para estar operativo en 45 minutos.

# Buscador de Ofertas ITtude v1.0

Un sistema de búsqueda laboral impulsado por IA, construido para Claude Code + Cowork. 18 skills, 4 sub-agentes, datos insider de entrevistas para empresas LATAM y globales, y un briefing matutino diario que maneja tu búsqueda en 20-30 minutos.

Desarrollado por [ITtude](https://ittude-agile.com) — Acelera tu carrera como líder de productos digitales.

## Para Quién Es

- **Product Managers** y **Product Owners** en cualquier nivel (Junior PM hasta VP/CPO)
- **Profesionales en transición a PM** desde consultoría, project managers, scrum masters, analistas, ingeniería, diseño, investigación u otras funciones

Los datos insider y los frameworks de entrevista están orientados a roles de producto. El motor central (adaptación de CV, networking, prep de entrevista, negociación) detecta automáticamente transiciones de carrera y activa el modo career-changer cuando el usuario no tiene títulos PM previos.

## Qué Incluye

```
buscador-ofertas-ittude/
├── CLAUDE.md              # Prompt del sistema - Claude lo lee automáticamente
├── configuracion/                 # Guía de instalación + checklist de primera sesión
├── .claude/skills/        # 18 skills (CV, entrevistas, networking, etc.)
├── biblioteca-contexto/       # Tus datos personales (experiencia, plan de carrera, targets)
├── tareas-cowork/          # Prompt del briefing matutino diario para Cowork
├── plantillas/             # Templates de CV, trabajo muestra, prototipo
├── sub-agentes/            # 4 agentes revisores (reclutador, ATS, HM, entrevistador)
├── datos-insider/          # Intel de entrevistas para empresas LATAM + frameworks
└── briefings/             # Outputs del briefing diario
```

## Inicio Rápido

1. Abrí esta carpeta en tu editor (VS Code, Cursor, o cualquier terminal)
2. Iniciá Claude Code en la terminal: `claude`
3. Ejecutá: `Leer CLAUDE.md y resumir qué hace este Buscador de Ofertas ITtude`
4. Seguí la guía de setup: `Leer configuracion/guia-instalacion.md`

## Probalo Ahora (Sin Setup)

Pegá cualquier descripción de puesto y ejecutá `/evaluar-oferta`. Descubrí si vale tu tiempo en 60 segundos — red flags, estimación salarial, intel de entrevista. No necesita biblioteca de contexto.

## Primera Sesión (~45 min)

Tres partes — contexto, targeting y tu primer briefing:

1. **Contexto (20 min):** `Ayudame a construir mi biblioteca de experiencias` → `Ayudame a completar el doc de Q&A maestro` → `Ayudame a completar mi plan de carrera`
2. **Targeting (15 min):** `/investigar-empresa generar lista de targets` → Revisar y reordenar ~100 empresas
3. **Primer briefing (10 min):** Configurar el briefing matutino, ejecutarlo y verificar la calidad del output

Ver `configuracion/checklist-primera-sesion.md` para el checklist completo.

## Uso Diario (20-30 min)

Tu briefing matutino entrega: top roles puntuados y rankeados, CVs adaptados, borradores de outreach, seguimientos y coaching del pipeline. Revisás, enviás, listo.

## Los 18 Skills

| Skill | Qué Hace |
|-------|---------|
| `/evaluar-oferta` | Pegá cualquier oferta, descubrí si vale tu tiempo en 60 segundos. Sin setup. |
| `/adaptar-cv` | CV adaptado desde experiencia real con score de cobertura |
| `/puntuar-oferta` | Puntuar ofertas de 1-100 en 5 dimensiones |
| `/investigar-empresa` | Research de empresas o generar lista de targets |
| `/solicitud-conexion` | 25 solicitudes de conexión personalizadas en LinkedIn |
| `/pedir-referido` | Secuencia completa de referido con identificación del HM |
| `/contactar-reclutador` | Mensaje al hiring manager liderando con trabajo muestra |
| `/trabajo-muestra` | 1-pager de análisis + prompt de prototipo |
| `/carta-presentacion` | Top 3 experiencias mapeadas a los top 3 requisitos |
| `/auditar-linkedin` | Optimización del perfil contra las ofertas objetivo |
| `/rastrear-postulaciones` | Tracker de pipeline con auto-actualizaciones |
| `/preparar-entrevista` | Paquete de prep desde web + datos insider |
| `/simular-entrevista` | Mock interactivo con calificación por las Tres Leyes |
| `/debrief-entrevista` | Análisis post-entrevista con reescrituras |
| `/nota-agradecimiento` | Nota personalizada desde transcripción |
| `/investigar-salario` | Datos de compensación de mercado con fuentes |
| `/negociar` | Análisis de oferta + lenguaje de contraoferta |
| `/retro-semanal` | Análisis de performance con coaching |

## Actualizaciones

Tus archivos de biblioteca-contexto nunca son sobreescritos por las actualizaciones. Verificar el número de versión en CLAUDE.md.

## Soporte

¿Preguntas? Contactá a [ITtude](https://ittude-agile.com).
