# WCAG 2.4.1: Saltar contenido

## Solución

Reemplazar las etiquetas `<span>` por las etiquetas semánticas de encabezado apropiadas

```javascript
[...]
<h1 className='text-4xl font-bold w-full text-center'>Compra final</h1>
{/* Counter */ }
<div className="w-full max-w-md mx-auto my-4">
  <div className='flex flex-col md:flex-row w-full md:space-x-8 py-4'>
    <section className='flex-1'>
      <h2 className='text-3xl font-bold mb-4'>Detalles del pago</h2>
      <div className='flex flex-row space-y-2'>
        <div className='flex-1'>
          <h3 className='text-2xl font-bold'>Dirección</h3>
          <address className='not-italic'>
            <p>{user.selectedLocation.address}</p>
            <p>{user.selectedLocation.neighborhood}</p>
            <p>{user.selectedLocation.name}</p>
          </address>
        </div>
        <div className='flex-1'>
          <h3 className='text-2xl font-bold'>Tarjeta</h3>
          <p>{'**' + user.selectedCreditCard.number.slice(-4)}</p>
          <p>
            <time dateTime={"01-" + user.selectedCreditCard.expiration_month + "-" + user.selectedCreditCard.expiration_year}>

              [...]

            </section>
            <section className='flex-1'>
              <h2 className='text-2xl font-bold'>Productos</h2>
              <div className='flex flex-col space-y-4 py-4 w-full md:h-64 md:overflow-auto'>

              [...]
```
