# WCAG 1.2.1: Entrevista con transcripción

## Solución

Añadir la respectiva transcripción de la entrevista

```javascript
{/* Transcripción de la entrevista */}
<h4 className='text-2xl font-semibold mb-4'>Transcripción</h4>
{transcriptParagraphs.map((paragraph, index) => (
  <p key={index} className='text-base mb-4'>
    {paragraph}
  </p>
))}
```
