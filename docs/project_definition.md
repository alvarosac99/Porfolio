# Definición del Proyecto: Portfolio Personal

Este documento define las bases, estructura de información, diseño visual y funcionalidades del portfolio personal de Álvaro Sebastián Acosta, basado en el diseño conceptual.

## 1. Bases del Proyecto

El proyecto consiste en un sitio web personal tipo portfolio, diseñado para mostrar el perfil profesional, habilidades y proyectos de un desarrollador multiplataforma. La estética principal gira en torno a un concepto "tech/dev", utilizando tipografías monoespaciadas y referencias a entornos de desarrollo (terminales, código).

### Objetivos Clave
- **Presentación Profesional:** Mostrar claramente el perfil "Full Stack / Multiplataforma".
- **Identidad Visual Fuerte:** Uso de un sistema de temas personalizado (Console, Favorite, Favorite Light).
- **Experiencia de Usuario (UX):** Navegación fluida, diseño responsivo y micro-interacciones atractivas.

### Stack Tecnológico
- **Framework:** Astro (Static Site Generator / Islands Architecture).
- **Estilos:** TailwindCSS (Integrado en Astro) o CSS Vanilla (Scoped).
- **Animaciones:** SVG inline, Canvas API, librerías ligeras (Motion One o similar si es necesario).
- **Fuentes:** Google Fonts (via @fontsource/package).
- **Despliegue:** Cloudflare Pages (Prioritario), Netlify o Vercel.

---

## 2. Arquitectura de la Información

El contenido se estructura en una sola página (One Page) con secciones claramente definidas, facilitando el escaneo rápido de la información.

### Secciones Principales
1.  **Header (Cabecera):**
    *   Logo/Marca personal.
    *   Navegación (Menú links o Icono hamburguesa en móvil).
2.  **Hero Section (Inicio):**
    *   Saludo: "> hola, soy".
    *   Nombre: "Álvaro Sebastián Acosta".
    *   Rol: "Desarrollador Multiplataforma".
    *   Descripción corta: Pasión por Linux, Docker, servidores y desarrollo web.
    *   Imagen/Visual: Composición gráfica o foto.
3.  **Stats (Estadísticas):**
    *   Contadores rápidos (ej. Años de experiencia, Proyectos, etc.).
4.  **Proyectos (Projects):**
    *   Grid de tarjetas de proyectos destacados.
5.  **Experiencia (Experience):**
    *   Línea de tiempo o lista de roles previos.
6.  **Aptitudes (Skills):**
    *   Categorías: Lenguajes, Sistemas, Herramientas, Habilidades personales.
7.  **Educación (Education):**
    *   Tarjetas con formación académica.
8.  **Intereses (Personal):**
    *   **Música:** Playlist o referencias a gustos musicales.
    *   **Videojuegos:** Mención a pasiones gaming.
9.  **Contacto (Contact CTA):**
    *   Llamada a la acción clara: "¿trabajamos juntos?".
    *   Correo electrónico visible: `acostacortizasalvarosebastian@gmail.com`.
    *   Botones de redes sociales.
    *   **Nota:** No se incluye número de teléfono por privacidad.
10. **Footer (Pie de página):**
    *   Copyright, enlaces legales o repetición de redes.

---

## 3. Temas y Diseño Visual

El diseño cuenta con un sistema de **tres temas principales**, permitiendo una experiencia personalizada.

### Tipografía
El uso de fuentes monoespaciadas es constante para reforzar la identidad de "desarrollador".
-   **Títulos / Acentos:** `JetBrains Mono` (Bold).
-   **Cuerpo / Textos:** `IBM Plex Mono` (Regular/Light).

### 1. Tema Console
Referencia directa a entornos de desarrollo y terminales.
-   **Fondo:** Oscuro (`#0C0C0C`).
-   **Animación:** Fondo interactivo SVG "Particle Constellation" (red de partículas).
-   **Acentos:** Verde menta / Turquesa (`#00D4AA`).
-   **Estilo:** Técnico, "Hacker", crudo.

### 2. Tema Favorito (Dark)
La estética personal preferida del usuario.
-   **Fondo:** Tonos oscuros profundos y gradientes sutiles (`#0C0C0C` / `#1A1520`).
-   **Acentos:** Naranja vibrante (`#FF7A42`).
-   **Estilo:** Moderno, cálido y elegante en modo oscuro.

### 3. Tema Favorito (Claro)
Versión luminosa del tema favorito.
-   **Fondo:** Blancos suaves y cremas (`#FAF8F6` / `#F0ECE8`).
-   **Acentos:** Naranja quemado (`#E8612A`).
-   **Estilo:** Limpio, minimalista y legible.

---

## 4. Funcionalidades de la Página

### 4.1. Navegación Responsiva
-   **Desktop:** Barra de navegación superior fija o estática.
-   **Móvil:** Header simplificado con botón "Hamburguesa" (`≡`) que despliega un **Menú Overlay** a pantalla completa (con botón de cierre `✕`, enlaces y redes sociales).

### 4.2. Selector de Temas (Theme Switcher)
-   Control para alternar entre **Console**, **Favorito** y **Favorito (Claro)**.
-   El tema "Console" activa funcionalidades específicas (animación de fondo).
-   Persistencia de la preferencia del usuario (localStorage).

### 4.3. Formulario de Contacto (Overlay/Modal)
-   Un componente interactivo para "Enviar correo".
-   Campos: Nombre, Asunto, Mensaje.
-   Feedback visual al enviar.
-   **Privacidad:** NO se solicita ni muestra número de teléfono.

### 4.4. Animación de Fondo (Concepto)
-   **Efecto:** "Particle Constellation". Red de partículas que reacciona al movimiento del cursor.
-    **Tecnología:** SVG o Canvas.
-   **Exclusividad:** Principalmente visible en el tema "Console", aunque podría adaptarse sutilmente a otros si se desea.

### 4.5. Micro-interacciones
-   **Hover effects:** Cambios de color/borde en tarjetas de proyectos y botones.
-   **Cursor:** Posibilidad de un cursor personalizado o efectos reactivos.
