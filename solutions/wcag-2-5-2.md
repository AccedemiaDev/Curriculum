# WCAG 2.5.2: Cancelar compra

## Solución

Se debe eliminar el trigger `onMouseDown` del botón de pago y solamente dejar el trigger `onClick`:

```javascript
<button
  onClick={handlePayment}
  className='h-9 w-48 bg-blue-dark text-white text-xl hover:bg-blue-darkest'>
  Comprar
</button>
```
