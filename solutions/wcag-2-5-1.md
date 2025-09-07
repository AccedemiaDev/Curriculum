# WCAG 2.5.1: Carrusel de imágenes

## Solución

Para realizar un carrusel de imágenes mas accesible, se debe de realizar las siguientes acciones:

- Añadir botones que permitan la navegación del carrusel.
- Los indicadores del númeral de la imágen deben ser convertidos a elementos `<button>` para que sean interactivos.
- El carrusel debe de ser posible de navegar mediante los botones de navegación:

```javascript
{/* Navigation buttons */ }
{
  index !== 0 &&
  <button
    onClick={goToPrevious}
    className='absolute left-0 top-1/2 transform -translate-y-1/2 bg-white bg-opacity-80 rounded-full p-1 mx-2 focus:outline-2 focus:outline-blue-dark'
    aria-label="Imagen anterior"
  >
    <ChevronLeft />
  </button>
}

// [...]

{
  index !== images.length - 1 &&
  <button
    onClick={goToNext}
    className='absolute right-0 top-1/2 transform -translate-y-1/2 bg-white bg-opacity-80 rounded-full p-1 mx-2 focus:outline-2 focus:outline-blue-dark'
    aria-label="Imagen siguiente"
  >
    <ChevronRight size={24} />
  </button>
}

// [...]

<div className="absolute bottom-2 left-0 right-0 flex justify-center gap-2">
  {images.map((_, i) => (
    <button
      key={i}
      className={`h-2 w-2 rounded-full ${i === index ? 'bg-blue-dark' : 'bg-white bg-opacity-60'}`}
      onClick={() => setIndex(i)}
      aria-label={`Ir a imagen ${i + 1}`}
      aria-current={i === index ? 'true' : 'false'}
    />
  ))}
</div>
```
