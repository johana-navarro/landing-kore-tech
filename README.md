# PFO1 — Landing de Portafolio Personal

Landing page de portafolio profesional desarrollada con **HTML semántico** y **CSS puro** (sin frameworks ni JavaScript).

## 🔗 Enlaces

- **Deploy en Vercel:** [URL pendiente]
- **Perfil de GitHub:** [github.com/johana-navarro](https://github.com/johana-navarro)

## 📄 Descripción

Sitio web de una sola página que presenta mi perfil profesional, habilidades técnicas, proyectos destacados, metodología de trabajo y un formulario de contacto. Diseñado con enfoque mobile-first y estética dark mode.

## 🎨 Decisiones de Diseño

### Tipografía
- **Outfit** (Google Fonts) para headings: tipografía geométrica y moderna que transmite solidez técnica.
- **Inter** (Google Fonts) para cuerpo de texto: alta legibilidad en pantalla, ideal para contenido profesional.
- Escala tipográfica fluida con `clamp()` para adaptación automática entre dispositivos.

### Paleta de colores
- **Modo oscuro elegante ("Dark Mauve")**: Base `#3a3238` con acentos en tono rosa/malva (`#d282a6` y `#e8b4bc`). Transmite profesionalismo, tecnología y estética contemporánea.
- Variables CSS (`--color-*`) para consistencia y fácil mantenimiento en toda la página.
- Formulario de contacto integrado con servicio real de mensajería **Formspree** (sin necesidad de JavaScript).

### Layout
- **CSS Grid** para layouts bidimensionales: sección de habilidades (4 columnas) y proyectos (2 columnas). Grid permite distribución uniforme y `auto-fit` con `minmax()` para responsividad intrínseca.
- **Flexbox** para alineación unidimensional: navegación, hero, metodología (3 pilares en fila), footer. Flexbox es más eficiente cuando la distribución es en un solo eje.
- La combinación de ambas tecnologías permite aprovechar las fortalezas de cada una según el contexto del componente.

### Responsive
- Enfoque **mobile-first**: estilos base para pantallas pequeñas, ampliados con media queries en `768px` y `1024px`.
- Unidades relativas (`rem`, `%`, `clamp()`, `auto-fit`) en lugar de valores fijos en píxeles.
- Menú hamburguesa implementado con CSS puro (checkbox hack), sin JavaScript.

### Interactividad
- Transiciones suaves en botones, cards y links de navegación.
- Animaciones personalizadas con `@keyframes`:
  - `fadeInUp`: entrada del contenido del hero.
  - `gradientShift`: fondo animado del hero con degradado.
  - `floatOrb`: orbes decorativos flotantes.
  - `scrollPulse`: indicador de scroll.
- Respeto por `prefers-reduced-motion` para accesibilidad.

### Accesibilidad
- Atributos `alt` descriptivos en todas las imágenes.
- Roles ARIA: `aria-label`, `aria-labelledby`, `aria-hidden`, `role="banner"`, `role="main"`, `role="contentinfo"`.
- Labels explícitos (`<label for="...">`) en todos los campos del formulario.
- Navegación semántica con `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`.

## 🤖 Declaración de Uso de IA

### Herramienta utilizada
- **Antigravity (Claude)** — Plan gratuito.

### Para qué la usé
- **Planificación**: generación del plan de implementación, estructura de secciones y sistema de diseño CSS.
- **Contenido textual**: redacción y refinamiento del texto de las secciones profesionales.
- **Código base**: generación del HTML semántico y CSS con variables, animaciones y responsive design.
- **Revisión de accesibilidad**: sugerencias de atributos ARIA y mejores prácticas.

### Experiencia previa
Tengo experiencia previa trabajando con herramientas de IA generativa para tareas de desarrollo, documentación técnica y testing en proyectos reales (TITANIUMgenIA, rediseño web B2B, QA de APIs REST).

### Qué revisé y adapté con criterio propio
- **Estructura y contenido**: toda la definición de secciones, proyectos y habilidades fue diseñada por mí basándome en mi experiencia real.
- **Paleta y tipografía**: seleccioné y ajusté colores y fuentes según mi criterio estético y el tono profesional buscado.
- **Código generado**: revisé la semántica HTML, corregí la estructura de ARIA, y adapté el CSS responsive a mis necesidades específicas.
- **Textos**: edité y personalicé todos los textos para que reflejen fielmente mi perfil y experiencia.

## 🛠️ Tecnologías e Identidad

- **HTML5 Semántico**: Estructura accesible con ARIA roles, Favicon con isologo rosa (`logo-r.png`) e identidad de pestaña `Kore Tech Solutions`.
- **CSS3 Puro**: Sistema de diseño responsive (Variables, Grid, Flexbox y Animaciones CSS sin frameworks).
- **Google Fonts**: Tipografías corporativas Outfit (headings) e Inter (body).
- **Formspree**: Integración real del formulario de contacto directa a email sin necesidad de JavaScript.
