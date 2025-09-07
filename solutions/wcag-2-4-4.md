# WCAG 2.4.4: "Leer mas" sobre noticias

## Solución

Cada pre-visualización a las publicaciones del blog debe de contener una entrada al contenido textual de la publicación acompañado del respectivo hipervínculo con la leyenda "Leer más".

```javascript
<h2 className='text-2xl font-bold mb-2'>{title}</h2>
<p className='text-lg mb-4'>{getSubstring(content, 150)}</p>
<a
  title={'Leer más sobre ' + title}
  href={'/blog/post' + (id + 1)}
  className='flex items-center justify-center h-9 w-28 bg-blue-dark text-white text-xl mt-3 hover:bg-blue-darkest'>Leer más</a>
```
