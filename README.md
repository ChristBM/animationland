# Animationland
Es un pequeño juego con solo HTML5 y CSS3 en el cual pongo en práctica mis habilidades para el dibujo y animación con CSS3. Es un proyecto que viene de un reto del curso de animaciones con CSS de Platzi.

## ¿Cómo se juega?
Muy sencillo es intentar seleccionar los conejos hasta que tengas 4 en el Score.

## Propiedades de CSS usadas:
El contenedor padre: ```position: relative;``` y los hijos usan: ```position: absolute;```. Con esto logro que todos los hijos referencien sus posiciones al contenedor padre.

El otro tema importante es el de crear capas(contexto de apilamiento). Para diferenciar las posiciones en Z de cada elemento le asigno varios valores de ```z-index: #;``` de 1 en adelante del contenedor más lejano al más cercano.

Para alinear los contenedores se usa: ```top: #px;```, ```bottom: #px;```, ```left: #px;```, ```right: #px;```. Con esto los posiciono en el eje (x;y) del elemento padre.

Para permitir que los contenedores salgan de sus padres y no se vea o no ocurra un scroll feo, empleo las propiedades: ```overflow-y: hidden;``` y ```overflow-x: hidden;```. Esto ayuda a las animaciones que se ejecutan de manera infinita a entrar y salir del contenedor.

Para ahorrar el uso de etiquetas ```<div></div>``` a la hoa de dibujar elementos en CSS, empleo los pseudo-elementos ```::before``` y ```::after``` y dentro de cada uno la propiedad: ```content: '';``` Esta me permite duplicar el contenedor de la clase en cuestión y modificarlo a mi gusto.(ver clases:```.ojos {...}``` y ```.orejas {...}```)

Otra propiedad interesante y muy versátil es ```clip-path: polygon();```. Esta nos ayuda a crear máscaras de recorte o simplemente figuras de diferente tipo(círculos, polígonos, triángulos, elipses, etc.)

Para recrear el agua y el césped uso la propiedad ```background: linear-gradient();```, nos permite experimentar y dibujar diferentes patrones con CSS.

Por último está el  tema de las animaciones que era el objetivo principal de este ejercicio. ```animation: [name] [duration] [timing-function] [delay] [iterationcount] [direction] [fill-mode] [play-state];``` y los key-frames ```@keyframes name {}```. Es importante seleccionar bien que propiedades animar para tener una buena performance.

## Recursos y Enlaces
[Tipografía utilizada](https://www.dafont.com/es/another-danger.font)

[SVGs](https://svgsilh.com/)

[Dibuja con CSS](https://dev.to/raulmar/no-tengas-miedo-a-dibujar-con-css-1ck)

[Patrones con CSS](https://dev.to/cchana/explained-creating-a-zigzag-pattern-with-just-css-13g1)

[Generador de Patrones](https://www.magicpattern.design/tools/css-backgrounds)

[Dibuja con un solo div](https://a.singlediv.com/)

[clip-path:](https://developer.mozilla.org/es/docs/Web/CSS/clip-path)

[Generador de clip-path](https://bennettfeely.com/clippy/)

[Aprende a crear una máscara de recorte en CSS](https://platzi.com/blog/aprende-a-crear-mascaras-de-recorte-con-css/)

[::after](https://developer.mozilla.org/es/docs/Web/CSS/::after)

[::before](https://developer.mozilla.org/es/docs/Web/CSS/::before)


## Contribuyendo
El código está disponible para el que desee lo modifique y lo use a su conveniencia. Espero que les sirva para aprender algo más de CSS3.
Atenderé las solicitudes de modificaciones para mejorarlo siempre y cuando usemos solo HTML5 y CSS3.

## Licencia

[MIT](https://choosealicense.com/licenses/mit/)