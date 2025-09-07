# WCAG 1.2.2: Anuncio con subtítulos

## Solución

Añadir el respectivo archivo de subtítulos dentro del elemento `<video>`

```javascript
<track
  src={subtitlesUrl}
  kind="subtitles"
  srcLang="es"
  label="Español"
  default
/>
```
