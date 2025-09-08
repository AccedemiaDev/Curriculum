# WCAG 2.5.1: Carrusel de imágenes

## Descripción

Este criterio de éxito busca garantizar que las páginas web incluyan gestos simples y accesibles para interactuar con los elementos, evitando gestos complejos o múltiples puntos de contacto.

Esto implica que las acciones importantes, como deslizar o tocar, deben ser posibles con un solo gesto simple. Por ejemplo, un botón debe activarse con un solo toque en lugar de requerir un gesto de arrastre. Estas prácticas benefician especialmente a personas con discapacidades motoras o limitaciones físicas, al facilitar la interacción con la página web.

## Caso

Al visualizar cada uno de los productos disponibles en el catálogo de CompraFácil, es posible observar que estos vienen acompañados con un carrusel de imágenes que permiten al cliente visualizar las imágenes de un producto si este contiene mas de una imágen, siendo la única manera de desplazar la colección de imágenes arrastrando el puntero para acceder a la siguiente imágen.

Esta implementación presenta serias dificultades para usuarios con limitaciones motoras que no pueden realizar gestos precisos de arrastre, así como para quienes utilizan tecnologías de asistencia como punteros de cabeza o control por teclado. Al no ofrecer alternativas como botones de navegación (anterior/siguiente) que puedan activarse con un solo clic o pulsación, estos usuarios quedan efectivamente excluidos de poder ver todas las imágenes de los productos, limitando su capacidad para tomar decisiones informadas de compra.

## Criterio de éxito

Cualquier funcionalidad que requiera que se active una ruta táctil (ejemplo: arrastrar con el dedo en una pantalla táctil) también necesita un método alternativo que facilite la interacción de quienes no pueden realizar el gesto (ver criterios completos).

## Mas información

[Understanding SC 2.5.1: Pointer Gestures (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/pointer-gestures)
[Carousel (Slide Show or Image Rotator) Pattern](https://www.w3.org/WAI/ARIA/apg/patterns/carousel/)
