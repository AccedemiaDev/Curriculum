# WCAG 2.2.1: Contador para pago

## Solución

Es posible añadir un botón que permita extender la duración del contador por 30 minutos

```javascript
// Add 30 minutes to timer (up to max 3 hours)
const extendTime = () => {
  setTimeLeft(prevTime => {
    const newTime = prevTime + extensionTime
    return newTime <= maxTime ? newTime : maxTime
  })
}

[...]

<button
  onClick={extendTime}
  className="px-4 py-2 bg-blue-dark text-white rounded hover:bg-blue-darkest transition-colors"
  disabled={timeLeft + extensionTime > maxTime}>
  Añadir 30 minutos
</button>
```
