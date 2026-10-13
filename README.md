# ROALDIX Technologies — Landing Page

Landing page corporativa de **ROALDIX Technologies**, empresa tecnológica con sede en México enfocada en la prestación de servicios tecnológicos, desarrollo y venta de software a medida, soluciones web e informatización de procesos para empresas y organizaciones tanto a nivel nacional como internacional.

## 🎯 Propósito

Servir como canal digital principal para captar clientes potenciales, presentar la identidad institucional y el catálogo integral de servicios tecnológicos de la empresa, explicar la metodología de trabajo y ofrecer un canal directo y validado para solicitar cotizaciones y consultas a través de WhatsApp y correo electrónico.

---

## 📋 Secciones de la Página

| # | Sección | Identificador | Descripción |
|---|---|---|---|
| 0 | **Navbar** | `#topNavbar` | Barra de navegación fija con efecto glassmorphism, logotipo corporativo, enlaces a secciones, selector bilingüe (ES / EN) y botón de acceso rápido al formulario. |
| 1 | **Hero** | — | Mensaje central: *"Empresa que transforma ideas en soluciones digitales"*, insignias de innovación tecnológica, etiquetas de servicios clave y botones CTA para explorar servicios o enviar consulta por WhatsApp. |
| 2 | **¿Quiénes somos?** | `#nosotros` | Resumen institucional, propósito empresarial, tarjetas con la **Misión** (soluciones confiables y funcionales) y **Visión** (marca referente de innovación), acompañadas de imagen ilustrativa del equipo. |
| 3 | **Impacto en tu Negocio** | `#impacto` | Tres beneficios cuantificables para los clientes: *Optimización Operativa*, *Reducción de Costos* y *Escalabilidad Comercial*. |
| 4 | **Nuestros Valores** | — | Seis pilares fundamentales: *Innovación*, *Calidad*, *Compromiso*, *Adaptabilidad*, *Transparencia* y *Confidencialidad*. |
| 5 | **Servicios Tecnológicos** | `#servicios` | Catálogo de **9 servicios especializados**: <br>1. Desarrollo y venta de software<br>2. Diseño y desarrollo web<br>3. Desarrollo de aplicaciones móviles<br>4. Inteligencia artificial e informatización<br>5. Pruebas y calidad de software (QA)<br>6. Mantenimiento y soporte de software<br>7. Bases de datos e integración de sistemas<br>8. Seguridad informática<br>9. Consultoría y asesoría tecnológica |
| 6 | **Metodología** | — | Proceso estructurado en 6 etapas: *01 Análisis* → *02 Planificación* → *03 Diseño* → *04 Desarrollo* → *05 Pruebas* → *06 Entrega*. |
| 7 | **¿Por qué elegirnos?** | `#sectores` | Cinco ventajas competitivas: soluciones a la medida, resultados prácticos, escalabilidad a futuro, comunicación clara y tecnología con propósito. |
| 8 | **Sectores que apoyamos** | `#sectores` | Sectores clave atendidos: *Comercio y distribución*, *Servicios profesionales*, *PyMEs*, *Agroindustria* y *Emprendimientos digitales*. |
| 9 | **Preguntas Frecuentes** | `#faq` | 5 preguntas clave con respuestas sobre alcance de software, requisitos de solicitud, cálculo de costos, plazos de entrega y optimización de sistemas heredados. |
| 10 | **Formulario de Consulta** | `#contacto` | Formulario interactivo con validación estricta en tiempo real para cotizaciones directas hacia WhatsApp. |
| 11 | **Canales de Contacto** | `#contacto` | Tarjetas con enlaces directos para Email (`info@codecoresystems.com`), WhatsApp directo (`+52 323 196 0575`) y ubicación en México. |

---

## 🛠️ Stack Tecnológico

El proyecto está desarrollado utilizando estándares web modernos con enfoque en rendimiento, accesibilidad y máxima compatibilidad:

### 1. Frontend & Marcado
- **HTML5 Semántico**: Uso riguroso de etiquetas semánticas (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<form>`, `<select>`).
- **CSS3 Vanilla**:
  - **Custom Properties (Variables CSS)** para consistencia cromática, espaciados y radios de borde.
  - **Flexbox y CSS Grid** para maquetación adaptable en múltiples columnas.
  - **Glassmorphism y Backdrop Filter** (`backdrop-filter: blur()`).
  - **Gradientes y Acentos Neón** con sombras de resplandor (`box-shadow: 0 0 ...`).
  - **Animaciones y Transiciones CSS** (micro-animaciones `@keyframes fadeInError`, efectos hover y elevaciones).
  - **Scrollbar personalizada** con diseño integrado a la paleta visual.

### 2. Lógica & Interactividad (JavaScript Vanilla ES6+)
- **Validación Heurística y de Formato en el Formulario**:
  - Restricción de tipeo en tiempo real (`beforeinput` e `input`) que impide escribir caracteres no permitidos en el teléfono.
  - Validación de campos requeridos antes de la apertura de WhatsApp (Nombre, Servicio, Teléfono, Correo y Mensaje).
  - Comprobación de formato de correo con expresión regular estándar (`RFC-compliant regex`).
  - Validación de teléfono: longitud mínima de 8 dígitos y sanitización automática de caracteres y posición del prefijo `+`.
  - Limpieza reactiva de errores visuales conforme el usuario escribe o cambia opciones.
- **Integración con WhatsApp Click-to-Chat**:
  - Codificación segura de parámetros URI (`encodeURIComponent`) para generar el mensaje preformateado y estructurado con todos los datos del lead.
- **Scroll Suave Sincronizado**:
  - Navegación interna por anclas vinculada al contenedor con scroll personalizado (`#pageScroll`).

### 3. Internacionalización (i18n)
- **Sistema i18n Nativo en JavaScript**:
  - Soporte bilingüe completo: **Español (ES)** e **Inglés (EN)**.
  - Traducción dinámica sin recargar la página mediante atributos `data-i18n` y `data-i18n-placeholder`.
  - Cobertura total de traducciones: títulos, descripciones, opciones del desplegable, etiquetas, placeholders y mensajes de error del formulario.

### 4. Recursos Externos & CDN
- **Google Fonts**: Tipografías **Outfit** (títulos, encabezados y logotipos) e **Inter** (cuerpo de texto y párrafos de alta legibilidad).
- **Font Awesome 6.4.0 (CDN)**: Conjunto de iconos vectoriales para acciones, estados y tarjetas de servicios.

### 5. Optimización para Motores de Búsqueda (SEO) y Redes Sociales
- **Datos Estructurados Schema.org (JSON-LD)**: Tipo `ProfessionalService` con catálogo de ofertas `OfferCatalog`, teléfono, dirección, horario de atención y correo.
- **Open Graph (Facebook, LinkedIn, WhatsApp)**: Metaetiquetas completas (`og:title`, `og:description`, `og:image`, `og:locale`, `og:url`).
- **Twitter Cards**: Formato `summary_large_image`.
- **Etiquetas de idioma e indexación**: `robots`, `googlebot`, `canonical`, etiquetas `alternate` con `hreflang` (`es`, `en`, `x-default`).

---

## 📱 Diseño Responsivo

Diseño totalmente adaptable a cualquier resolución con breakpoints definidos:
- **Desktop Extra Ancho (>1200px)**: Grid de 3 y 4 columnas con navegación completa.
- **Desktop y Laptop (1024px – 1200px)**: Adaptación a 2 y 3 columnas.
- **Tablet y Móvil (<768px)**:
  - Navegación optimizada.
  - Conversión de grids a una sola columna para garantizar legibilidad.
  - Formulario adaptado a pantalla completa sin desbordamiento.
  - Acciones táctiles optimizadas con áreas de pulsación cómodas.

---

## 📂 Estructura del Proyecto

```
landing_page_roaldix_tecnologies/
├── index.html              # Archivo principal (Estructura HTML, CSS y JS integrados)
├── README.md               # Documentación general del proyecto
└── img/                    # Recursos gráficos y multimedia
    ├── logo_fondo_blanco.jpg   # Logotipo corporativo e icono favicon
    └── about_tech.jpg          # Fotografía ilustrativa de la sección institucional
```

---

## 🚀 Despliegue y Ejecución

La página no requiere compiladores ni dependencias externas; se puede ejecutar en cualquier entorno:

1. **Localmente**: Abrir el archivo `index.html` directamente en cualquier navegador web.
2. **Servidor HTTP local**:
   ```bash
   # Con Python
   python -m http.server 8080

   # Con Node.js (npx)
   npx serve .
   ```
3. **Producción**: Compatible con plataformas de alojamiento estático como GitHub Pages, Vercel, Netlify, Cloudflare Pages o cualquier servidor web (Nginx / Apache).

---

© 2026 ROALDIX Technologies. Todos los derechos reservados.
