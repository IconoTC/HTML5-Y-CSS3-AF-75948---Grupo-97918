# HTML - CSS

HTML5 Y CSS3 AF 75948 - Grupo 97918
Fecha inicio: 01/06/2026
Fecha fin: 05/06/2026
Horario: 9:00 - 14:00

- Instructor: Alejandro Cerezo Lasne <alce65@hotmail.es>
- Repositorio: <https://github.com/IconoTC/HTML5-Y-CSS3-AF-75948---Grupo-97918.git>

## Temario original

- HTML. 
    - Arquitectura de aplicaciones Web. 
    - El lenguaje HTML. 
    - Estructura básica de un documento HTML. 
    - Organización de texto. 
    - Hipertexto: links HTML. 
    - Imágenes. 
    - Tablas. 
    - La entrada de usuario. Formularios. 
    - Interacción con CSS. 
    - Interacción con JavaScript. 
- HTML5. 
    - Compatibilidad de los navegadores. 
    - Artículos, secciones, cabeceras. 
    - Nuevos componentes de formulario. 
    - Audio. 
    - Video. 
    - Otras APIs de intercambio de información. 
- CSS3. 
    - Arquitectura, propósito y alcance de CSS. 
    - Inclusión de elementos CSS en páginas HTML5. 
    - Hojas de estilo, reglas y propiedades. 
    - Herencia de estilos: resolución de conflictos. 
    - Tratamiento de textos. 
    - Gestión de imágenes. 
    - Organización de tablas. 
    - Definición de la estructura de una página HTML5. 
    - Transformaciones, transiciones y animaciones.

## Desarrollo

### Dia 1 (Lunes 01/06/2026)

- Presentación formador y alumnos. Curso
- Requisitos técnicos
  - Navegador web actualizado (Google Chrome, ...)
  - Editor de código (Visual Studio Code, ...)
  - Repositorio GitHub
    - Documentación
    - Recursos y tools
- Introducción a HTML
  - Arquitectura de aplicaciones Web
  - El lenguaje HTML (demo-01)
    - Etiquetas y atributos
    - Hipertexto: links HTML
    - Imágenes
    - Comentarios

[descanso]

- Validación y estructura de un documento HTML (demo-02)
  - Elementos imprescindibles y recomendables
  - Documentos HTML5_ html, head, body
  - Etiquetas más usadas: p, h1-h6, a, img, div, span

- HTML en la Web (demo-03)
  - Interacción con CSS
  - Interacción con JavaScript

- Elementos del head (demo-04)
  - Metadatos
  - Título de la página
  - Enlaces a recursos externos: favicon, CSS, JavaScript, fuentes, ... 
  - Metadatos para SEO y redes sociales

- Revisión del estándar HTML. Clasificación de etiquetas. 

### Dia 2 (Martes 02/06/2026)

- Etiquetas principales de HTML (demo-05): Porfolio

- Semántica en HTML5 y roles Aria
- Sectioning:
-   - `<header>`: Encabezado de una sección o página.
    - `<footer>`: Pie de página o sección.
    - `<main>`: Contenido principal de la página (etiqueta de grouping).
    - headings: `<h1>` a `<h6>`: Títulos y subtítulos de secciones.
    - `<hgroup>`: Agrupación de encabezados y párrafos relacionados.
    - `<nav>`: Contenedor de enlaces de navegación.
    - `<section>`: Agrupación temática de contenido.
    - `<article>`: Contenido independiente y autocontenible.
    - `<address>`: Información de contacto del autor o propietario de la página.

- roles aria y aria-label
- header y footer en secciones y artículos
- uso de clases y css para cambiar la estética de los elementos semánticos (e.g. headings)
- validación de la estructura

Otras etiquetas:
  - grouping
    - listas: `<ul>`, `<ol>`, `<li>`
    - párrafos: `<p>`
    - `<div>`: Contenedor genérico sin significado semántico específico (etiqueta de grouping).
- enlaces (anchor): `<a>`: enlaces externos o internos a la página

[descanso]

- Otras etiquetas de sectioning y grouping
  - `<aside>`: Contenido relacionado pero separado del contenido principal.
  - `<menu>` 
  - `<dl>`, `<dt>` and `<dd>`
  - `<hr>` 
  - `<pre>` 
  - `<blockquote>`

- Text formatting:
  - `<strong>`: Texto importante.
  - `<em>`: Texto enfatizado.
  - `<small>`: Texto de menor importancia.
  - ...

- Embedding content:
  - `<img>`: Incrustación de imágenes en la página.
  - `<figure>` and `<figcaption>` 
  - `<iframe>`: Incrustación de otra página web dentro de la actual.
  - `<iframe>`: Videos de YouTube.
  - `<video>`: Reproducción de video.
  - `<audio>`: Reproducción de audio.

- Nueva página 'contactos': enlaces entre páginas
- Formularios:
  - `<form>`: Contenedor para elementos de formulario.
  - `<input>`: Campos de entrada de datos.
  - `<textarea>`: Área de texto multi-linear.
  - `<select>`: Menú desplegable.
  - `<button>`: Botón interactivo.
  - `<label>`: Etiqueta para elementos de formulario.

### Dia 3 (Miércoles 03/06/2026)

- Tablas en html
  - `<table>`: Contenedor para una tabla de datos.
  - `<tr>`: Fila de la tabla.
  - `<th>`: Celda de encabezado de la tabla.
  - `<td>`: Celda de datos de la tabla.

- Elementos interactivos y multimedia
  - De otros tipos: `<a>`, `<button>` (diferencioias), `<input>` ...     
  - `<details>`: Contenido adicional que el usuario puede mostrar u ocultar.
  - `<summary>`: Resumen o título para el contenido de `<details>`.
  - `<dialog>`: Diálogo modal o ventana emergente.
  - JS: in-line v. scripts internos o externos

- CSS
  - Concepto de CSS: propósito,
  - Inclusión de CSS en HTML: inline, interno, externo 
  - Arquitectura de CSS: selectores, propiedades, valores, reglas, hojas de estilo

[descanso]

- Selectores CSS
  - Selectores básicos: por etiqueta, clase, id
  - Selectores de agrupación y descendencia
  - Alternativa actual: anidamiento (nesting) de selectores
  - Selectores de atributos
  - Pseudo-clases y pseudo-elementos

- Especificidad y herencia de estilos
  - Reglas de especificidad: inline > id > clase > etiqueta
  - Herencia de estilos: cómo los estilos se propagan a través del árbol DOM
  - Resolución de conflictos: cómo se aplican los estilos cuando hay múltiples reglas que coinciden

### Dia 4 (Jueves 04/06/2026)

- Elementos del lenguaje CSS
  - Pseudo-elementos: 
    - `::first-letter`, 
    - `::first-line`,
    - `::before`, 
    - `::after`,
    - `::marker`,
  - Pseudo-clases: 
    - `:target`,
    - `:hover`, 
    - `:focus`, 
    - `:nth-child()`, ...

  - Variables y funciones CSS
    - Variables CSS: `--nombre-variable`
    - Funciones CSS: `calc()`, `var()`, `rgb()`, ...
    - Paletas de colores
    - Escala de tamaños para la tipografía
    - Guías de estilo (Style Guides)
    - Hojas de CSS básicas

[descanso] 11:10 - 11:40

- Elementos del lenguaje CSS (continuación)
  - Unidades de medida en CSS
    - Absolutas: `px`, `cm`, `mm`, `in`, `pt`, `pc`
    - Relativas: `%`, `em`, `rem`, `vw`, `vh`, `vmin`, `vmax`
    - Rem vs Em
  
- Diseño (Layout) de páginas web con CSS
  - Box model: contenido, padding, border, margin
    - Box-sizing: content-box vs border-box
  - Display: block, inline, inline-block, none
  - Layouts clásicos: float, clear, inline-block
  - Flexbox: diseño flexible para contenedores y elementos hijos


### Dia 5 (Viernes 05/06/2026)

- Diseño (Layout) de páginas web con CSS
  - Grid: diseño de cuadrícula para organizar elementos en filas y columnas 

[descanso] 11:00 - 11:30

- Encuesta: <https://forms.cloud.microsoft/pages/responsepage.aspx?id=tA7tEz6_F0GYpeEuIOyC74dmltakDyZNkCB0fAWABS1UMlpRT1VPTUhFVlEwNzY0NkExUldORDZINSQlQCNjPTEkJUAjdD1n&route=shorturl>

- Position: static, relative, absolute, fixed & anchors

- Responsive Web Design (RWD)
  - Media queries: diseño adaptativo para diferentes tamaños de pantalla
  - Enfoques de diseño:
    - Mobile-first
    - Desktop-first
    - Mobile-only
  - Mobile-first design: enfoque de diseño que prioriza la experiencia móvil
    - Menus hamburguesa
  - CSS Dinámico
    - Transformaciones, transiciones y animaciones
  - Theme selector solo con CSS: has()
  - Recortes de imágenes: shape-outside