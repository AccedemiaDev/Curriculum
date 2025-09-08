# WCAG 3.2.1: Redirección de inicio de sesión

## Solución

Se debe eliminar el atributo `onFocus`, el cual es el que realiza una redirección a la página para iniciar sesión si el elemento `<a>` recibe un enfoque.

```html
<a href='/login'
  className='flex items-center justify-center bg-blue-light h-full px-3 font-semibold text-lg rounded-md hover:bg-blue-medium-light'>
  Iniciar sesión
</a>
```
