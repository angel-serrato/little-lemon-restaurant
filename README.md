<h1 align="center">🍋 Little Lemon Restaurant</h1>

<div align="center">
  <p>Sitio web promocional para Little Lemon Restaurant - Cocina mediterránea auténtica con diseño responsive y moderno.</p>
</div>

---

## 📋 Tabla de Contenidos

- [Vista General](#-vista-general)
- [Características](#-características)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Diseño y Estilos](#-diseño-y-estilos)
- [Instalación y Uso](#-instalación-y-uso)
- [Estructura del Código](#-estructura-del-código)
- [Responsive Design](#-responsive-design)

---

## 🎯 Vista General

Little Lemon Restaurant es un sitio web promocional desarrollado con HTML5 y CSS3 puro, diseñado para presentar el restaurante de cocina mediterránea y sus servicios. El proyecto implementa las mejores prácticas de desarrollo web moderno con un enfoque en la experiencia del usuario y diseño responsive.

### Características Principales del Proyecto

- ✅ **Diseño 100% responsive** adaptado a todos los dispositivos
- ✅ **Sin dependencias de JavaScript** - HTML y CSS puro
- ✅ **Metodología BEM** para organización CSS
- ✅ **Tipografías escalables** con clamp()
- ✅ **Sistema de diseño con CSS Variables**
- ✅ **Animaciones y transiciones** suaves
- ✅ **Optimización SEO** con meta tags apropiados
- ✅ **Imágenes optimizadas** desde Unsplash CDN

---

## ✨ Características

### Secciones del Sitio

1. **Header con Navegación**

   - Logo del restaurante
   - Menú de navegación con 4 enlaces (Home, Menu, About Us, Contact)
   - Efectos hover interactivos

2. **Banner Promocional**

   - Promoción destacada: "30% Off This Weekend!"
   - Imagen de fondo con overlay oscuro
   - Efecto hover con zoom sutil

3. **Sección de Features (3 cards)**

   - **Menu**: Información sobre platos de temporada
   - **Book a table**: Reservas online
   - **Opening hours**: Horario de atención (11:00 AM - 11:00 PM)
   - Cada card incluye imagen, título y descripción
   - Animaciones hover con elevación y sombras

4. **Footer**
   - Logo del restaurante
   - Copyright © 2025 Little Lemon

### Interactividad Visual

- Hover effects en todos los elementos interactivos
- Transiciones suaves (0.3s ease)
- Scale effects en navegación
- Elevación de cards con transform: translateY()
- Sombras dinámicas

---

## 📁 Estructura del Proyecto

```
little-lemon-restaurant/
│
├── index.html          # Estructura HTML principal
├── style.css          # Estilos CSS con metodología BEM
└── README.md          # Documentación del proyecto
```

---

## 🛠 Tecnologías Utilizadas

### Core

- **HTML5** - Estructura semántica
- **CSS3** - Estilos y animaciones

### Fuentes (Google Fonts)

- **Merriweather Sans** - Encabezados
- **Signika Negative** - Subtítulos
- **ABeeZee** - Texto del cuerpo

### Recursos Externos

- [Unsplash](https://unsplash.com/) - Imágenes de alta calidad
- [ImgBB](https://ibb.co/) - Hosting de logos

---

## 🎨 Diseño y Estilos

### Sistema de Colores

```css
--color-primary-yellow: #fdd835        /* Amarillo primario */
--color-primary-variant-yellow: #f9a825 /* Variante amarillo */
--color-secondary-green: #388e3c        /* Verde secundario */
--color-text-dark: #212121              /* Texto oscuro */
--color-text-light: #ffffff             /* Texto claro */
--color-background: #ffffff             /* Fondo */
```

### Tipografía Escalable

El proyecto utiliza la función `clamp()` para tipografía fluida y responsive:

```css
--text-h1: clamp(2.0736rem, 1.6734rem + 1.7785vw, 3.0518rem)
--text-h2: clamp(1.728rem, 1.4362rem + 1.2971vw, 2.4414rem)
--text-h3: clamp(1.44rem, 1.2301rem + 0.933vw, 1.9531rem)
--text-h4: clamp(1.2rem, 1.0517rem + 0.6591vw, 1.5625rem)
--text-paragraph: clamp(1rem, 0.8977rem + 0.4545vw, 1.25rem)
```

### Sistema de Espaciado

```css
--spacing-1: 4px
--spacing-2: 8px
--spacing-3: 12px
--spacing-4: 16px
--spacing-6: 24px
--spacing-8: 32px
```

### Metodología BEM

El CSS sigue la convención Block-Element-Modifier:

```css
.header                  /* Block */
.header__logo           /* Element */
.header__nav            /* Element */
.header__nav-link       /* Element */
.header__nav-link:hover /* Modifier (pseudo-clase) */
```

---

## 💻 Instalación y Uso

### Requisitos Previos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Editor de código (opcional, para modificaciones)

### Pasos de Instalación

1. **Clonar o descargar el repositorio**

   ```bash
   git clone <repository-url>
   cd little-lemon-restaurant
   ```

2. **Abrir el proyecto**
   - Opción 1: Hacer doble clic en `index.html`
   - Opción 2: Usar Live Server en VS Code
   - Opción 3: Servir con cualquier servidor local

### Uso con Live Server (VS Code)

```bash
# Si tienes Live Server instalado
# Click derecho en index.html > Open with Live Server
```

### Personalización

1. **Cambiar colores**: Editar variables CSS en `:root` en `style.css`
2. **Modificar contenido**: Editar texto en `index.html`
3. **Cambiar imágenes**: Reemplazar URLs en `index.html`

---

## 📐 Estructura del Código

### HTML Semántico

```html
<header>    <!-- Navegación principal -->
<main>      <!-- Contenido principal -->
  <section class="banner">      <!-- Promoción -->
  <section class="features">    <!-- Características -->
    <article> ... </article>    <!-- Cards individuales -->
</main>
<footer>    <!-- Pie de página -->
```

### CSS Reset

El proyecto incluye un CSS reset completo (Meyer's Reset) para consistencia cross-browser.

### Organización CSS

1. **Reset CSS** (líneas 1-135)
2. **Variables CSS** (líneas 136-162)
3. **Header Styles** (líneas 163-205)
4. **Main Content** (líneas 206-280)
5. **Footer Styles** (líneas 281-305)
6. **Media Queries** (líneas 306-353)

---

## 📱 Responsive Design

### Breakpoints

```css
/* Mobile First - Base styles */
@media (min-width: 576px) {
  /* Small tablets */
}
@media (min-width: 768px) {
  /* Tablets */
}
@media (min-width: 992px) {
  /* Small desktops */
}
@media (min-width: 1200px) {
  /* Desktops - Layout horizontal */
}
@media (min-width: 1400px) {
  /* Large screens */
}
```

### Comportamiento Responsive

- **Mobile (< 1200px)**: Layout vertical en columna
- **Desktop (≥ 1200px)**:
  - Layout horizontal de 3 columnas para features
  - Ancho máximo de 900px centrado
  - Gap de 2rem entre elementos

---

## 🎯 Buenas Prácticas Implementadas

✅ **Semántica HTML5**: Uso de tags como `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`

✅ **Accesibilidad**:

- Alt text en todas las imágenes
- Estructura de encabezados lógica
- Contraste de colores apropiado

✅ **SEO**:

- Meta description descriptiva
- Viewport meta tag para móviles
- Charset UTF-8

✅ **Performance**:

- CSS crítico inline (Google Fonts)
- Imágenes optimizadas con parámetros Unsplash
- Sin JavaScript innecesario

✅ **Mantenibilidad**:

- Metodología BEM
- CSS Variables para theming
- Código bien comentado y organizado

---

## 🚀 Mejoras Futuras

Posibles mejoras para futuras versiones:

- [ ] Agregar formulario de reservas funcional
- [ ] Implementar galería de imágenes del menú
- [ ] Añadir página de menú completo
- [ ] Integrar sistema de reviews
- [ ] Añadir mapa de ubicación
- [ ] Implementar modo oscuro
- [ ] Agregar animaciones avanzadas con JavaScript
- [ ] Optimizar para Core Web Vitals

---

## Contact

- Website [serrato.me](https://serrato.me/)
- GitHub [@angel-serrato](https://github.com/angel-serrato)
- LinkedIn [/in/angel-serrato/](https://www.linkedin.com/in/angel-serrato/)

<div align="center">
  <p>Desarrollado con ❤️ para Little Lemon Restaurant</p>
  <p>© 2025 Little Lemon. Todos los derechos reservados.</p>
</div>
