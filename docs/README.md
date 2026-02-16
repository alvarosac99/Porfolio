# Definición del Proyecto: Portfolio Personal

Este documento define las bases, estructura de información, diseño visual y funcionalidades del portfolio personal de Álvaro Sebastián Acosta, basado en el diseño conceptual.

## 1. Bases del Proyecto

El proyecto consiste en un sitio web personal tipo portfolio, diseñado para mostrar el perfil profesional, habilidades y proyectos de un desarrollador multiplataforma. La estética principal gira en torno a un concepto "tech/dev", utilizando tipografías monoespaciadas y referencias a entornos de desarrollo (terminales, código).

### Objetivos Clave
- **Presentación Profesional:** Mostrar claramente el perfil "Full Stack / Multiplataforma".
- **Identidad Visual Fuerte:** Uso de temas contrastantes (Consola vs. Claro) para reflejar versatilidad.
- **Experiencia de Usuario (UX):** Navegación fluida, diseño responsivo y micro-interacciones atractivas.

### Stack Tecnológico Sugerido (Basado en notas de diseño)
- **Frontend:** HTML5, CSS3 (Vanilla o Tailwind), JavaScript (Vanilla).
- **Animaciones:** SVG inline, Canvas API (para efecto de partículas), CSS transitions.
- **Fuentes:** Google Fonts (JetBrains Mono, IBM Plex Mono).

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
    *   Contadores rápidos (ej. Años de experiencia, Proyectos, etc. - *contenido placeholder en diseño*).
4.  **Proyectos (Projects):**
    *   Grid de tarjetas de proyectos destacados.
5.  **Experiencia (Experience):**
    *   Línea de tiempo o lista de roles previos.
6.  **Aptitudes (Skills):**
    *   Categorías: Lenguajes, Sistemas, Herramientas, Habilidades personales.
7.  **Educación (Education):**
    *   Tarjetas con formación académica.
8.  **Contacto (Contact CTA):**
    *   Llamada a la acción clara: "¿trabajamos juntos?".
    *   Correo electrónico visible: `acostacortizasalvarosebastian@gmail.com`.
    *   Botones de redes sociales.
9.  **Footer (Pie de página):**
    *   Copyright, enlaces legales o repetición de redes.

---

## 3. Temas y Diseño Visual

El diseño cuenta con un sistema de temas dual, permitiendo al usuario alternar entre una estética oscura (default) y una clara.

### Tipografía
El uso de fuentes monoespaciadas es constante para reforzar la identidad de "desarrollador".
-   **Títulos / Acentos:** `JetBrains Mono` (Bold).
-   **Cuerpo / Textos:** `IBM Plex Mono` (Regular/Light).

### Tema Consola (Dark Mode)
Inspirado en IDEs y terminales modernas.
-   **Fondo:** Tonos muy oscuros (`#0C0C0C`, `#0E0C10`, `#141414`).
-   **Acentos:**
    -   Turquesa/Verde menta (`#00D4AA`).
    -   Naranja vibrante (`#FF7A42`).
-   **Texto:** Blanco (`#FAFAFA`) y Gris azulado (`#8B939F`).
-   **Bordes/Líneas:** Gris oscuro sutil (`#1E2028`).

### Tema Claro (Light Mode)
Una versión limpia y minimalista, manteniendo la estructura.
-   **Fondo:** Blancos y cremas (`#FFFFFF`, `#FAF8F6`, `#F0ECE8`).
-   **Acentos:**
    -   Naranja quemado (`#E8612A`).
-   **Texto:** Negro suave (`#1A1118`) y Gris topo (`#6B5F65`).
-   **Bordes/Líneas:** Gris claro (`#D8D0D5`).

---

## 4. Funcionalidades de la Página

### 4.1. Navegación Responsiva
-   **Desktop:** Barra de navegación superior fija o estática.
-   **Móvil:** Header simplificado con botón "Hamburguesa" (`≡`) que despliega un **Menú Overlay** a pantalla completa (con botón de cierre `✕`, enlaces y redes sociales).

### 4.2. Cambio de Tema (Theme Switcher)
-   Capacidad de alternar instantáneamente entre el Tema Consola y el Tema Claro.
-   Persistencia de la preferencia del usuario (localStorage).

### 4.3. Formulario de Contacto (Overlay/Modal)
-   Un componente interactivo para "Enviar correo".
-   Campos: Nombre, Asunto, Mensaje.
-   Feedback visual al enviar.

### 4.4. Animación de Fondo (Concepto)
-   **Efecto:** "Particle Constellation". Red de partículas que reacciona al movimiento del cursor.
-    **Tecnología:** SVG o Canvas.
-   **Comportamiento:** Las partículas se conectan cuando están cerca, creando formas geométricas dinámicas.

### 4.5. Micro-interacciones
-   **Hover effects:** Cambios de color/borde en tarjetas de proyectos y botones.
-   **Cursor:** Posibilidad de un cursor personalizado o efectos reactivos (según el concepto de partículas).
