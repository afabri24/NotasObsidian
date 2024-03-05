Validar pedido

El administrador se encuentra en la *administración del pedido* y **visualiza los pedidos pendientes por validar** y cuando **selecciona uno se le muestra** *aceptar pedido*, donde se encuentran los detalles del pedido, el estado y los botones de confirmación. El administrador seleccionara aceptar y el **sistema cambiara el estado del pedido** en la *tabla de pedidos*, **notificara al cliente por correo** y **muestra al administrador un mensaje de afirmación**.

1. El sistema se muestra la pantalla de administración de pedidos
2. El administrador selecciona un pedidos
3. El sistema muestra la pantalla aceptar pedido donde se encuentran, los detalles del pedido, el estado y los botones de confirmación.
4. El administrador da click en el botón aceptar
5. El sistema guarda el nuevo estado del pedido en tabla de los pedidos, recupera el correo del cliente de la tabla clientes y envía un correo del estado del pedido al cliente del pedido
6. El administrador recibe un mensaje de afirmación del estado del pedido

Flujo alterno:

FA01:El administrador selecciona la opción rechazar en la pantalla aceptar pedido
	4.1 El administrador da click en el botón de rechazar
	5.1 El sistema mostrara un formulario para ingresar datos necesarios para el rechazo del pedido
	6.1 El administrador llenara el formulario con los datos y da click en boton enviar.
	7.1 El sistema cambiara el estado del pedido, envia un correo al cliente y muestra un mensaje de afirmacion.

Excepción:

EX01: El sistema no pudo guardar el estado del pedido por que no se pudo conectar a la base de datos
	6. El administrador recibe el un mensaje de error con un texto de "intentarlo nuevamente"
	7. El sistema seguirá mostrando la pagina de administración de pedidos

---
Visualizar productos

El usuario se encuentra en la pagina principal, donde se le mostraran todos los productos de la base datos


----
Añadir Producto

El administrador se encuentra en la pagina de administración de productos, donde agregara uno nuevo, se abrira la pantalla de agregar producto donde pondra todos los datos basicos para agregarlo, despues la pantalla cambiara a caracteristicas del producto y agregara los datos que guste el administrador agregar y por ultimo finalizara la accion, agregando el producto a tabla productos y por ultimo el administrador podra ver un mensaje de afirmacion.


1. El sistema muestra la pagina administracion de producto.
2. El usuario da click en el boton agregar.
3. El sistema lo redirecciona  a la pagina agregar pedido, donde se le mostrara el formulario de datos necesarios.
4. El usuario agregara los datos necesarios y presionara el boton siguiente.
5. El sistema lo redireccionara a un formulario donde podra agregar datos extras y/o caracteristicas del producto a agregar
6. El usuario agrega los datos y presionara el boton siguiente.
7. El sistema le mostrara los detalles del producto 
8. El usuario presionara agregar producto.
9. El sistema guarda el producto nuevo en la tabla productos, redirige al usuario al  y le muestra al administrador un mensaje de afirmacion.

Flujo alterno:

FA01: Omitir paso de agregar datos extras
	 4.1. El administrador da click en omitir datos extra.
	 5.1 El sistema guardara los datos que fueron ingresados en la pantalla datos basicos en un nuevo producto en la tabla productos, redireccionara al usuario a la pagina administracion productos y mostrara un mensaje de afirmacion de producto guardado
FA02: Cancelar operacion
	4.2. El administrador dara click en el boton Cancelar
	4.3 El sistema lo redireccionara al paso 1 sin hacer ninguna accion extras

Excepciones:

EXEC1: No hubo conexión a la base de datos al agregar producto
	7.El sistema mostrara un mensaje donde le pedirá que lo intente de nuevo mas tarde
	8. El usuario se encontrara en la pagina anterior