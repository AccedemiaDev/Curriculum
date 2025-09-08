# WCAG 4.1.2: Blob no legible

## Solución

Es posible utilizar el parámetro `aria-hidden` para ocultar de los lectores de pantalla el elemento gráfico

```javascript
<img 
  src={blobSvg} aria-hidden="true" 
  className='w-80 h-80 md:h-108 md:w-108 lg:h-128 lg:w-128'/>
```
