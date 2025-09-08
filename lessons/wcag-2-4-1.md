# WCAG 2.4.1: Saltar contenido

## Descripción

Este criterio de éxito busca garantizar que los usuarios puedan navegar por una página web de manera lógica y predecible, utilizando encabezados y etiquetas descriptivas.

Esto implica que los encabezados y etiquetas deben reflejar claramente el propósito de los elementos que describen. Por ejemplo, un encabezado de sección debe indicar claramente el contenido que sigue, y una etiqueta de formulario debe describir adecuadamente el campo correspondiente. Estas prácticas benefician especialmente a personas con discapacidades visuales o cognitivas, al facilitar la navegación y comprensión del contenido.

## Caso

Dentro de la sección de pago, los títulos y subtítulos que conforman a la respectiva sección utilizan elementos etiquetas `<span>` en vez de las etiquetas semánticas de encabezado apropiadas como `<h1>`, `<h2>`, o `<h3>`.

Esta práctica, aunque visualmente pueda simular la apariencia de encabezados, priva a los usuarios de tecnologías de asistencia, como los lectores de pantalla, de la estructura jerárquica esencial para comprender y navegar el contenido. Sin encabezados semánticos, los usuarios no pueden saltar directamente a secciones de interés ni obtener un resumen rápido de la organización de la página, lo que resulta en una experiencia de navegación ineficiente, confusa y que no cumple con el objetivo de una navegación lógica y predecible.

## Criterio de éxito

Se debe proporcionar un tipo de control para que las personas puedan ignorar cierto contenido repetitivo (ejemplo: un menú de navegación).

## Mas información

[Understanding SC 2.4.1: Bypass Blocks (Level A)](https://www.w3.org/WAI/WCAG22/Understanding/bypass-blocks)
