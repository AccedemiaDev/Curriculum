# WCAG 1.4.1: Indicación de error

## Solución

Brindar de mas elementos decorativos al mensaje de error que permitan al usuario entender mucho mejor el contenido. En este caso es posible añadir un contorno y fondo rojo junto con texto en negrilla:

```javascript
<p
  ref={errorRef}
  tabIndex={-1}
  role="alert"
  className='bg-red-100 border border-red-400 text-red-700 px-4 py-3 rounded focus:outline-none focus:ring-2 focus:ring-red-500 font-bold'>
  {error}
</p>
```
