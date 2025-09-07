# WCAG 2.2.2: Anuncio parpadeante

## Solución

Es posible disminuir la duración del anuncio parpadeante a una cantidad igual o menor que cinco segundos

```javascript
// Effect to stop blinking after 5 seconds
  useEffect(() => {
    const timer = setTimeout(() => {
      setIsBlinking(false);
    }, 5000); // 5000 milliseconds = 5 seconds

    // Clean up timer on unmount
    return () => clearTimeout(timer);
}, []);
```
