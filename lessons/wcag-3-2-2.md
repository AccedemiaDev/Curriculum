# WCAG 3.2.2: Activación de inicio de sesión

## Descripción

Este criterio de éxito busca garantizar que los componentes interactivos de una página web, como menús y formularios, se comporten de manera consistente en todas las páginas.

Esto implica que los elementos interactivos deben mantener su ubicación y funcionalidad en todo el sitio web. Por ejemplo, un menú de navegación debe aparecer en el mismo lugar y con las mismas opciones en todas las páginas. Estas prácticas benefician especialmente a personas con discapacidades cognitivas o visuales, al facilitar la navegación y comprensión del contenido.

## Caso

Para entregar el formulario de inicio de sesión, el usuario debe de introducir sus credenciales. Una vez introducida la contraseña, dada una espera de 5 segundos el formulario será entregado de manera automática. Esta implementación causa problemas significativos para diversos usuarios, especialmente aquellos con discapacidades cognitivas o motoras que pueden necesitar más tiempo para verificar sus datos antes de enviarlos.

Al no requerir una acción explícita como hacer clic en un botón de "Iniciar sesión", el usuario pierde el control sobre cuándo enviar sus datos, y puede confundirse al ser redirigido inesperadamente, o peor aún, enviar credenciales incorrectas sin poder corregirlas a tiempo.

## Criterio de éxito

No deben ocurrir cambios contextuales que puedan desorientar a alguien cuando hay una interacción en un campo de entrada de datos (ejemplo: elementos de formulario), sin confirmación directa (ejemplo: un botón de confirmación).

## Mas información

[Understanding SC 3.2.2: On Input (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/on-input)
