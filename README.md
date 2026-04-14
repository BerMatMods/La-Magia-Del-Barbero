```markdown
# 💈 La Magia Del Barbero | Barber Shop Premium

<p align="center">
  <img src="https://i.postimg.cc/Z5Y5wLpy/Picsart-26-04-14-07-41-30-147.png" alt="La Magia Del Barbero - Logo Neón" width="220"/>
</p>

<p align="center">
  <strong>🐺 Estilo • Precisión • Esencia 🐺</strong>
</p>

<p align="center">
  <a href="https://wa.me/51977355999">
    <img src="https://img.shields.io/badge/💬_WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp"/>
  </a>
  <a href="https://www.facebook.com/share/1BHEnX7T2R/">
    <img src="https://img.shields.io/badge/📘_Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"/>
  </a>
  <a href="https://www.tiktok.com/@lamagiadelbarbero.5">
    <img src="https://img.shields.io/badge/🎵_TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white" alt="TikTok"/>
  </a>
  <img src="https://img.shields.io/badge/📍_Andahuaylas%2C%20Perú-gold?style=for-the-badge&logo=google-maps&logoColor=white" alt="Ubicación"/>
</p>

---

## 🐺 Identidad Visual & Branding

```yaml
🎨 Logo Principal:
   └─ Formato: PNG con fondo transparente
   └─ Estilo: Neón dorado sobre fondo oscuro
   └─ Ubicación: /head > link[rel="icon"] + footer
   └─ URL: https://i.postimg.cc/Z5Y5wLpy/Picsart-26-04-14-07-41-30-147.png

🖼️ Imagen Hero:
   └─ Fondo con overlay dorado y efecto parallax
   └─ URL: https://i.postimg.cc/Hs1LGmDV/1776171893e71a.png

🎭 Paleta de Colores CSS Variables:
   └─ --black: #050505          → Fondo base
   └─ --black-card: #0f0f0f     → Tarjetas
   └─ --gold: #D4AF37           → Acentos principales
   └─ --gold-light: #FFD700     → Gradientes hover
   └─ --gold-glow: rgba(...)    → Efectos de brillo
   └─ --white / --gray          → Tipografía

✒️ Tipografía:
   └─ Orbitron (700/900) → Títulos y logos
   └─ Rajdhani (300/500/700) → Cuerpo de texto
   └─ Carga: Google Fonts con preconnect
```

---

## 🏗️ Estructura del Proyecto

```
la-magia-del-barbero/
│
├── 📄 index.html                 # Archivo principal (single-page)
│
├── 🎨 <style>                    # CSS embebido en <head>
│   │
│   ├── 🎭 :root                  # Variables CSS globales
│   ├── 🌐 Reset & Base Styles   # Normalización y body
│   ├── ✨ Animaciones Keyframes # fadeInUp, pulse, bounce, gradientShift
│   ├── 📱 Responsive Media Queries # Mobile-first breakpoints
│   ├── 🧭 Header & Navigation   # Sticky header + menú móvil
│   ├── 🦸 Hero Section          # Full-viewport con background fijo
│   ├── 📦 Cards System          # Servicios y profesionales (grid)
│   ├── 📅 Booking System        # Formulario + confirmación WhatsApp
│   ├── 🗺️ Location Section      # Google Maps embed + contacto
│   ├── 🔻 Footer & Social       # Logo + redes + copyright
│   ├── 🪟 Modal System          # Advertencias y UX feedback
│   └── 📱 WhatsApp Float Button # Botón flotante con animación
│
├── ⚙️ <script>                   # JavaScript embebido antes de </body>
│   │
│   ├── 🔄 Scroll Optimization   # requestAnimationFrame para header
│   ├── 📱 Mobile Menu Toggle    # Hamburguesa + navegación responsive
│   ├── 📋 Form Validation       # Campos obligatorios + modal alerta
│   ├── 💬 WhatsApp Generator    # Construcción de mensaje con formato
│   ├── 📅 Date Formatting       # Parseo manual para evitar timezone
│   ├── 🎯 Smooth Scroll         # Navegación entre anclas
│   └── ♻️ Form Reset            # Limpieza y reutilización
│
└── 🖼️ Assets Externos (CDN/Postimg)
    ├── 🌐 Fonts: Google Fonts + Font Awesome 6.4.0
    ├── 🖼️ Imágenes: postimg.cc + Unsplash (lazy loading)
    └── 🗺️ Mapa: Google Maps Embed API
```

---

## 🛠️ Stack Tecnológico

<p align="center">
  <img src="https://img.shields.io/badge/📄_HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/🎨_CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/⚡_JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/🔤_Google_Fonts-4285F4?style=for-the-badge&logo=googlefonts&logoColor=white" alt="Google Fonts"/>
  <img src="https://img.shields.io/badge/🎯_Font_Awesome-339AF0?style=for-the-badge&logo=fontawesome&logoColor=white" alt="Font Awesome"/>
  <img src="https://img.shields.io/badge/🗺️_Google_Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Google Maps"/>
</p>

```diff
✅ Características Técnicas:
+ Single-Page Application (SPA) sin frameworks
+ CSS Variables para theming consistente
+ Backdrop-filter para efectos glassmorphism
+ CSS Grid + Flexbox para layouts responsivos
+ Animaciones nativas con keyframes optimizadas
+ Integración directa con WhatsApp Business API
+ Lazy loading en imágenes para performance
+ Meta tags SEO + Google Site Verification
+ Accesibilidad: aria-labels + contraste adecuado
+ Prefers-reduced-motion para accesibilidad
```

---

## 🧩 Componentes Principales

### 🧭 Header & Navegación
```html
<!-- Sticky header con backdrop-filter -->
<header id="mainHeader" class="scrolled">
  <nav>
    <!-- Logo con imagen + texto gradient -->
    <!-- Nav links desktop + mobile toggle -->
    <!-- Efecto hover con underline dorado animado -->
  </nav>
</header>
```

### 🦸 Hero Section
```css
/* Fondo con imagen fija + overlay gradient */
/* Badge dorado con box-shadow glow */
/* Título con background-clip: text gradient */
/* Botón CTA con animación shine on hover */
```

### 📦 Sistema de Tarjetas
```css
.service-card, .professional-card {
  /* Border dorado semi-transparente */
  /* Hover: translateY + scale image + glow shadow */
  /* Pseudo-elemento ::before para línea superior animada */
  /* Transiciones cubic-bezier para suavidad */
}
```

### 📅 Sistema de Reservas
```javascript
// Flujo completo:
1. Selección de servicio → scroll suave al formulario
2. Validación en tiempo real de campos requeridos
3. Generación de resumen con formato de fecha ES-PE
4. Construcción de mensaje WhatsApp con plantilla estructurada
5. Redirección automática a wa.me con texto codificado
6. Confirmación visual con animación de éxito
```

### 🪟 Modal de Advertencia
```css
/* Overlay con blur + animación de entrada */
/* Icono de alerta con pulse animation */
/* Botón de cierre accesible + tecla ESC */
/* Scroll automático al formulario tras cerrar */
```

---

## 📱 Responsive Design

```css
/* Breakpoint principal: 768px */
@media (max-width: 768px) {
  /* Menú hamburguesa con slide-down */
  /* Tipografía escalada para legibilidad */
  /* Grids convertidos a columna única */
  /* Botones full-width para toque fácil */
  /* WhatsApp float ajustado a pantalla pequeña */
  /* Imágenes profesionales con aspect-ratio 1:1 */
}
```

<p align="center">
  <img src="https://img.shields.io/badge/📱_Mobile_First-✅-green?style=for-the-badge" alt="Mobile First"/>
  <img src="https://img.shields.io/badge/🖥️_Desktop_Optimized-✅-blue?style=for-the-badge" alt="Desktop"/>
  <img src="https://img.shields.io/badge/♿_Accesibilidad-✅-purple?style=for-the-badge" alt="Accesibilidad"/>
</p>

---

## 🚀 Despliegue Rápido

```bash
# 🔹 Opción 1: GitHub Pages (Recomendado)
1. Subir index.html a repositorio público
2. Ir a Settings → Pages → Branch: main → /root
3. ¡Listo! Tu sitio estará en https://tu-usuario.github.io/repo

# 🔹 Opción 2: Servidor Local con VS Code
1. Instalar extensión "Live Server"
2. Click derecho en index.html → "Open with Live Server"
3. Acceso inmediato en http://127.0.0.1:5500

# 🔹 Opción 3: Hosting Estático (Netlify/Vercel)
1. Arrastrar carpeta del proyecto al dashboard
2. Configuración automática de build (none required)
3. Dominio personalizado opcional
```

---

## 🔧 Personalización

```css
/* 🎨 Cambiar colores de marca */
:root {
  --gold: #TU_COLOR;           /* Acentos principales */
  --gold-light: #TU_COLOR_LIGHT; /* Gradientes hover */
  --gold-glow: rgba(...);      /* Efectos de brillo */
}

/* 🖼️ Reemplazar logo */
<!-- Buscar en HTML y actualizar src -->
<img src="TU_URL_DE_LOGO.png" alt="Tu Marca">

/* 🗺️ Actualizar ubicación */
<!-- Reemplazar iframe de Google Maps -->
<iframe src="TU_EMBED_URL" ... ></iframe>

/* 💬 Cambiar número de WhatsApp -->
<!-- Buscar "51977355999" y reemplazar en: -->
- wa.me links
- JavaScript: profPhone variable
- Contact section
```

---

## 📄 Metadatos & SEO

```html
<meta name="description" content="Barbería profesional en Andahuaylas...">
<meta name="author" content="BerMatMods - Desarrollo Web">
<meta name="google-site-verification" content="JG8_KsOCw2MKItELjrA7vFLxZwO_NQsJsUs1s6prI8A" />
<link rel="icon" sizes="192x192" href="..."> <!-- PWA ready -->
<title>La Magia Del Barbero | Kennedy Ramirez</title>
```

---

## 🤝 Créditos & Licencia

```
© 2026 La Magia Del Barbero — Todos los derechos reservados.
🐺 Diseño y Desarrollo: BerMatMods - Desarrollo Web
🔗 Portfolio: https://bermatmods.github.io/BerMat-Code/

📜 Licencia: Uso exclusivo para el negocio "La Magia Del Barbero".
   Prohibida la reproducción total o parcial sin autorización escrita.
```

<p align="center">
  <a href="https://bermatmods.github.io/BerMat-Code/" target="_blank">
    <img src="https://img.shields.io/badge/©_𖤍_BERMA𝐓-CODE_𖤍-gold?style=for-the-badge&logo=github&logoColor=white" alt="BerMatMods"/>
  </a>
</p>

---

<p align="center">
  <strong>🐺 La Magia Del Barbero | Forjando Estilo con Esencia 🐺</strong>
</p>

<p align="center">
  <a href="#-la-magia-del-barbero--barber-shop-premium">
    <img src="https://img.shields.io/badge/⬆_Volver_Arriba-black?style=for-the-badge&logo=up&logoColor=gold" alt="Volver Arriba"/>
  </a>
</p>
```
