# Guía docente: portafolio HTML + CSS + SEO

**Nivel:** iniciación. **Herramientas:** VS Code, extensión Live Server y navegador.
**Objetivo didáctico:** cada alumno termina con su propio portafolio. No es obligatorio publicar el sitio.

## Cómo empezar
1. Descomprime el ZIP y abre la carpeta completa `portafolio_clase` en VS Code.
2. Abre `index.html` con Live Server (clic derecho > Open with Live Server).
3. Enseña primero el resultado visual. Después ve escribiendo el código con la clase en orden de bloques. El archivo final sirve de referencia, no para copiar sin comprender.
4. Los alumnos deben sustituir el nombre ficticio, textos, enlaces y proyectos.

## Bloque 1 — Estructura base HTML (30–40 min)
**Explica**: `<!DOCTYPE html>` (HTML5); `html lang="es"` (idioma); `head` (metadatos); `body` (visible); `charset` (tildes); `viewport` (móviles).
**Teclado**: crear una versión vacía de `index.html` con `head` y `body`. Añadir `h1` y un `p` de presentación.
**Comprobación**: abrir con Live Server; preguntar qué cambia en pestaña del navegador cuando editan `title`.

## Bloque 2 — HTML semántico (45–55 min)
**Explica**: `header` cabecera, `nav` navegación, `main` contenido principal, `section` bloque temático, `article` pieza independiente, `footer` pie. Explica por qué no conviene crear toda la página con `div`.
**Teclado**: construir cabecera, hero, Sobre mí, Habilidades, Proyectos y Contacto sin CSS. Introducir ID y anclas `href="#proyectos"`.
**Comprobación**: navegar al pulsar enlaces; debe existir un único `h1` principal y `h2` por sección.

## Bloque 3 — CSS inicial (40 min)
**Explica**: separar estructura (HTML) y presentación (CSS); selector, propiedad y valor. Relación `link rel="stylesheet"`; `color`, `background`, `font-family`, `margin`, `padding`, `border` y modelo de caja. `:root` contiene variables de colores.
**Teclado**: empezar con reglas para `body`, `h1`, `h2`, `.contenedor` y `.seccion`.
**Prueba**: cambiar `--principal` y observar el efecto general.

## Bloque 4 — Cabecera y hero (45–55 min)
**Explica**: clases (`class`), `display:flex` para menú, `display:grid` para dos columnas, `gap`, estilos de enlace y botón.
**Teclado**: construir los bloques `.barra`, `.menu`, `.hero-contenido`, `.boton`.
**Prueba**: quitar `display:grid` y observar el nuevo orden.

## Bloque 5 — Habilidades y proyectos (45 min)
**Explica**: tarjetas con `article`, imágenes locales (ruta relativa), `width`/`height`, texto `alt`, `loading="lazy"` y `object-fit`.
**Teclado**: agregar una tarjeta nueva de habilidad y una de proyecto con imagen propia. Crear una ficha HTML por proyecto (se incluyen dos ejemplos).
**Prueba**: ¿qué ocurre al escribir mal el nombre de la imagen?

## Bloque 6 — SEO aplicado (45–55 min)
**Explica**:
- `title`: nombre único y descriptivo de cada página; se muestra como título de pestaña y puede usarse en resultados de búsqueda.
- `meta name="description"`: resume cada página; puede usarse como fragmento en el buscador, pero no siempre.
- `html lang="es"`: idioma principal, útil para accesibilidad.
- `h1`, `h2`, `h3`: jerarquía comprensible; no insertar palabras clave de manera artificial.
- URL/rutas descriptivas: `proyectos/cafeteria.html` es más claro que `p1.html`.
- `alt`: describir imágenes informativas para accesibilidad; evitar sobrecargarlo con keywords.
- Enlaces internos: ayudan a navegar y descubrir páginas.
- `robots` no garantiza indexación; para aparecer en Google es necesario publicar un sitio rastreable y cumplir otros requisitos. No añadir una canonical ficticia en localhost.
**Prueba**: cambiar el título y la descripción de cada proyecto para que sean diferentes. Identificar una frase de búsqueda relevante, sin repetirla artificialmente.

## Bloque 7 — Responsive y accesibilidad (30–40 min)
**Explica**: `@media (max-width:760px)` cambia columnas; `max-width:100%` evita que imágenes sobresalgan; `:focus-visible` muestra el foco de teclado.
**Prueba**: herramientas de desarrollador > modo móvil; revisar a 375 px y escritorio. Navegar por Tab sin ratón.

## Preguntas para revisar en voz alta
1. ¿Por qué el texto de `<title>` no aparece como un título visible en la página?
2. ¿Cuál es la diferencia entre `section` y `article`?
3. ¿Qué significa `href="#contacto"` y qué debe existir para que funcione?
4. ¿Qué diferencia existe entre `class` e `id`?
5. ¿Por qué una descripción SEO no garantiza clics ni posicionamiento?
6. ¿Para qué sirve `alt` y en qué se diferencia del título de la imagen?
7. ¿Qué hace la media query en pantalla estrecha?
8. ¿Por qué usar títulos diferentes en páginas distintas?

## Entrega del alumno
Carpeta con `index.html`, `css/estilos.css`, `img/`, páginas de proyectos que enlacen correctamente, captura de escritorio y captura de móvil, y un texto breve explicando tres decisiones SEO (title, description, encabezados o enlaces internos).

## Nota docente
Las imágenes SVG incluidas son ilustraciones originales sencillas, no recursos externos. El nombre y correo son ficticios. Los enlaces de proyectos sí funcionan y abren fichas locales. No hay formulario porque sin servidor no enviaría mensajes. El botón de contacto abre el gestor de correo mediante `mailto:`.
