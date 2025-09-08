# WCAG 3.2.6: Botón de ayuda

## Descripción

Este criterio de éxito busca garantizar que los mecanismos de ayuda se presenten de manera consistente en todo el sitio web, facilitando que los usuarios puedan encontrar asistencia cuando la necesiten.

Esto implica que si se proporciona ayuda en una página, como información de contacto, formularios de asistencia o enlaces a FAQs, estos elementos deben aparecer en la misma ubicación y formato en todas las páginas donde estén disponibles. Estas prácticas benefician especialmente a personas con discapacidades cognitivas o de aprendizaje, al crear un patrón predecible que reduce la carga cognitiva y mejora la experiencia de usuario.

## Caso

Dentro de la barra de navegación, el enlace que redirige a la sección de ayuda solamente se encuentra disponible cuando el usuario se encuentra en la ruta raíz (`"/"`). Esta inconsistencia en la disponibilidad de la ayuda crea confusión significativa para los usuarios, especialmente aquellos con discapacidades cognitivas o de aprendizaje, que pueden haber memorizado la ubicación del enlace de ayuda en la página principal. 

Cuando navegan a otras secciones del sitio y necesitan asistencia, no encuentran el mecanismo de ayuda en la ubicación esperada, lo que aumenta su frustración y dificulta su capacidad para resolver problemas. Esta implementación contradice directamente el principio de consistencia y previsibilidad que facilita el uso efectivo de un sitio web, especialmente para usuarios con necesidades de accesibilidad.

## Criterio de éxito

Si se proporcionan algunas opciones de ayuda en una pantalla (ejemplo: datos de contacto humano), este mismo formato debe ser el mismo en todas las demás pantallas donde se proporciona ayuda.

## Mas información

[Understanding SC 3.2.6: Consistent Help (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/consistent-help.html)