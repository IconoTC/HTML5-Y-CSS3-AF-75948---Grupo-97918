dso# CSS Demo 01

Demo para probar selectores CSS. 

La estructura del documento se ha organizado en secciones temáticas. Se han añadido etiquetas `section` con el atributo `aria-label` para mejorar la accesibilidad y proporcionar una estructura más clara al documento. Las secciones incluidas son:

- header: Contiene el título principal de la página y la navegación.
- main: Contiene el contenido principal de la página, dividido en secciones para probar diferentes selectores CSS.
  - "Probando selectores"
    - "Subsección de prueba"
  - "Formulario de contacto"
- footer: Contiene el pie de página con información de copyright.

## Selectores CSS

Aunque no tiene especial efecto, se han agrupado las propiedades de CSS en @layer para organizar mejor el código. Las capas utilizadas son:

- Selectores básicos
  - Etiquetas HTML
  - Clases
  - IDs
- Otros selectors
  - Multiples selectores
  - Selectores de atributos
- Selectores combinados
  - Descendiente (espacio) (ver style.old.css)
  - Descendiente directo: (>) (ver style.old.css)
  - Anidamiento de descendientes: uso de &
  - Hermano adyacente: (+)
  - Hermano general: (~) 
- Selectores de estado
  - Pseudo-clases
  - Pseudo-elementos

## Especificidad

a -> important
b -> estilos inline
1 -> Ids
2 -> atributos, clases, pseudo-clases
3 -> elementos Y pseudo-elementos