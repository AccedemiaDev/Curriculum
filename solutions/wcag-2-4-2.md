# WCAG 2.4.2: Página de titulo dinámico

## Solución

Es posible realizar un mapeo dinámico para cada sección principal de CompraFácil, de tal manera que el título sea descriptivo con el contenido que se presenta:

```javascript
// Map component titles to their respective names
const titles = {
  catalog: 'Catalogo',
  blog: 'Blog',
  login: 'Iniciar Sesión',
  register: 'Registro',
  assistance: 'Asistencia',
  cart: 'Carrito de Compras',
  card: 'Tarjeta de Crédito',
  addcard: 'Agregar Tarjeta de Crédito',
  location: 'Ubicación',
  addlocation: 'Agregar Ubicación',
  payment: 'Método de Pago'
}

// Dynamic page component
function DynamicPage(props) {
  // Use either passed prop or URL parameter
  const params = useParams();
  const componentKey = (props.componentName || params.componentName || 'catalog').toLowerCase();

  const Component = components[componentKey] || Catalog;

  // Dynamically update the document title using the titles object
  useEffect(() => {
    const componentTitle = titles[componentKey] || 'CompraFácil'; // Fallback to "CompraFácil" if no title is found
    document.title = `${componentTitle}`;
  }, [componentKey]);

  return (
    <Background>
      <Component />
    </Background>
  );
}
```
