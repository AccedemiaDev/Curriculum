# WCAG 1.2.3: Presentación con audio descriptivo

## Solución

Añadir el respectivo archivo de audiodescripción dentro del elemento `<video>`

```javascript
<track
  src={audioDescriptionUrl}
  kind="descriptions"
  srcLang="es"
  label="Descripción de audio"
/>
```
