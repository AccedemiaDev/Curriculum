# WCAG 1.3.2: Orden lineal de navegación

## Solución

Remover las propiedades `flex-row reverse` y `space-x-reverse` del elemento `<navbar>`  y organizar la lista de enlaces al orden correcto:

```javascript
<nav>
  <ul className='flex items-center space-x-4'>
    <li className='text-white text-xl'>
      <a href='/'>Catálogo</a>
    </li>
    <li className='text-white text-xl'>
      <a href='/blog'>Blog</a>
    </li>
    <li className='text-white text-xl'>
      <a href='assistance'>Ayuda</a>
    </li>
  </ul>
</nav >
```
