# Skill: Estándares de Desarrollo Web (HTML5 & UX)

Este documento define las reglas obligatorias para la creación de interfaces web en este proyecto, asegurando calidad, accesibilidad y rendimiento.

## 1. Integridad Estructural y Sintaxis
- **Declaración <!DOCTYPE html>**: Todo archivo debe comenzar con esta etiqueta para activar el modo estándar de HTML5.
- **Jerarquía y Anidamiento Estrictos (LIFO)**: Los elementos deben cerrarse en el orden inverso al que se abrieron.
- **Uso de Minúsculas**: Todas las etiquetas y atributos deben escribirse en minúsculas por consistencia profesional.

## 2. Lógica Semántica (Adiós a la "Sopa de Divs")
- **Etiquetas con Significado**: Priorizar `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>` y `<footer>` sobre `<div>` y `<span>`.
- **Raíz de Títulos (H1)**: Un solo `<h1>` por página, usado para definir el tema principal, no para estilo visual.
- **Independencia con <article>**: Usar para bloques de contenido con sentido propio (posts, tarjetas de producto).

## 3. Accesibilidad (A11y)
- **Descripciones Alternativas (ALT)**: Todas las imágenes deben incluir el atributo `alt` descriptivo.
- **Vinculación Formulario-Etiqueta**: Los `<input>` deben tener un `id` vinculado al `for` de su `<label>`.
- **Roles ARIA**: Implementar `role` y `aria-label` para mejorar la experiencia con tecnologías asistivas.

## 4. Interacción y Experiencia de Usuario (UX)
- **Navegación Segura**: Enlaces con `target="_blank"` deben incluir `rel="noreferrer"` o `rel="noopener"`.
- **Teclados Optimizados**: Usar `type="email"`, `type="tel"`, `type="number"` para desplegar teclados móviles específicos.
- **Atributo Name**: Obligatorio en elementos de formulario para el procesamiento de datos en el servidor.

## 5. Estrategia de SEO y Metadatos
- **Metadatos Únicos**: Cada página debe tener un `<title>` (55-65 car.) y `<meta description>` (máx. 165 car.) únicos.
- **Enlaces Canónicos**: Usar `<link rel="canonical" href="...">` para evitar penalizaciones por contenido duplicado.

## 6. Rendimiento y Multimedia
- **Carga Diferida (Lazy Loading)**: Añadir `loading="lazy"` a imágenes fuera del área inicial de visualización.
- **Dimensiones Explícitas**: Definir `width` y `height` en imágenes para evitar el salto de diseño (layout shift).
