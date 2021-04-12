# clase 101
## UseEffect

Para continuar trabajando con APIs y UseEffect, nuestro proximo desafío será hacer una web que nos permita buscar y filtrar productos utilizando la API de Mercado Libre. 

Podés ver un ejemplo aquí, cortesía de una ex alumna de Ada :) https://meli-search.vercel.app/

La API de Mercado Libre se puede consultar en el siguiente endpoint: `https://api.mercadolibre.com/sites/MLA/search?q=busqueda` reemplazando "busqueda" por el término que quieras buscar. 


### Primera parte

Utilizando React, maquetá una web que tenga, como mínimo:

- Una barra de búsqueda en la parte superior. 
  -  La barra debe tener un `input` de tipo texto y un `submit` que deben estar rodeados de un `form`. 

Al enviar el formulario, debemos hacer un `fetch` a https://api.mercadolibre.com/sites/MLA/search?q=busqueda (reemplazando "busqueda" lo que el usuario haya escrito en el input) 

Una vez que funcione el fetch, maquetar debajo de la barra de navegación nna seccion con tarjetas que, 
  - Muestren el título de un producto. 
  - Muestren la foto del un producto.
  - Muestren el precio de un producto. 
  - Deben mostrar un camioncito si el producto tiene envío gratuito. 
  - Tengan un boton que diga "ver más".  

### Segunda parte

Al hacer click en el botón "ver más", debemos reemplazar toda la sección de tarjetas con los detalles de un producto. 

Entre los detalles se deben incluir, 
- Si el producto es nuevo o usado
- Cuantos productos se vendieron
- La foto del producto
- La descripcion del producto
- Titulo 
- Precio 
- Un botón "comprar" que lleve a la pagina de mercadolibre de ese producto en particular. 


### Tercera parte

Agrega filtros en la busqueda. Tras buscar un producto, el usuario verá todas las tarjetas. Sobre ellas, el usuario podrá elegir:
- Mostrar solo las que tienen envio gratuito. 
- Ordenar de mas cara a mas barata y viceversa. 
- Elegir solo los productos de determinada localidad. 
- Mostrar solo los productos de tiendas oficiales. 

### Cuarta parte


Hacé que tu web sea más accesible y placentera para el usuario. 
- En la esquina superior izquierda agrega un logo o imagen que lleve a la seccion principal de tu pagina (ningun producto mostrandose, ninguna busqueda en la barra de navegacion, la seccion principal vacia sin tarjetas, quiza con un mensaje que invite al usuario a buscar)
- Las tarjetas deben poder ser navegables con el teclado (puedo recorrer todas las tarjetas con `tab` y entrar al detalle de un producto con `enter`)
- La web debe ser responsive. 
