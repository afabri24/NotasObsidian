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

FA02: Cancelar operacion
	4.2. El administrador dara click en el boton Cancelar
	4.3 El sistema lo redireccionara al paso 1 sin hacer ninguna accion extra

Excepciones:

EXEC1: No hubo conexión a la base de datos al agregar producto
	7.El sistema mostrara un mensaje donde le pedirá que lo intente de nuevo mas tarde
	8. El usuario se encontrara en la pagina anterior

----
Hacer pedido

El Cliente se encuentra en un producto de su interés o se encontrara en su carrito de compras donde seleccionara realizar pedido donde podrá registrar como va pagar el pedido, después el cliente podrá crear una nueva dirección de envió o seleccionar una anteriormente creada, después podrá ver toda la información de su pedido donde podrá ver y podrá confirmar su pedido e inmediatamente se hará un pedido y le mostrara que su pedido esta en revisión

1. El sistema **muestra** la página de productos y carrito de compras.
2. El usuario **selecciona** un producto de interés o desde el carrito **elige** realizar pedido.
3. El sistema **redirige** al usuario a la página de pago, donde el usuario **registra** su método de pago.
4. El usuario **crea** una nueva dirección de envío o **selecciona** una dirección previamente registrada.
5. El sistema **muestra** un resumen del pedido con todos los detalles.
6. El usuario **revisa** la información del pedido y **confirma** la orden.
7. El sistema **registra** el pedido, **asigna** un estado de "en revisión" y **muestra** un mensaje de confirmación al usuario.
8. El usuario **visualiza** un mensaje de pedido realizado.

Flujo Alternativos:
(FA01): Cambiar el método de pago

3.1. El usuario **decide** cambiar el método de pago.
3.2. El sistema **permite** al usuario **seleccionar** un nuevo método de pago.
3.3. El usuario **elige** el nuevo método de pago y **continúa** al paso 4.

(FA01): Cambiar la dirección

3.1. El usuario **decide** cambiar la dirección.
3.2. El sistema **permite** al usuario **seleccionar** un nuevo método de pago.
3.3. El usuario **elige** el nuevo método de pago y **continúa** al paso 4.

(FA02): Cancelar el pedido

6.1. El usuario **decide** cancelar el proceso del pedido.
6.2. El sistema **muestra** una confirmación de cancelación.
6.3. El usuario **confirma** la cancelación.
6.4. El sistema **elimina** el proceso del pedido y **redirige** al usuario a la página de productos o cesta.

Excepciones:

EXC1: Error en el guardado del pedido

7.1. El sistema le da error en la conexión de la base de datos y por ello no se guarda el pedido
7.2. El usuario recibirá que hubo un error al hacer el pedido
7.3 el sistema le pedira que lo intente nuevamente en unos momentos o se contacte los administradores

____

1. El sistema **muestra** la página de administración de productos con la lista de productos existentes.
2. El usuario **selecciona** un producto de la lista y **elige** la opción de "Modificar".
3. El sistema **redirige** al usuario a la página de edición de producto, donde se **muestran** los datos actuales del producto.
4. El sistema **muestra** los detalles del producto a modificar.
5. El usuario **modifica** los datos del producto según sea necesario y **presiona** el botón "Guardar cambios".
6. El sistema **actualiza** el producto en la tabla de productos con los nuevos datos y **redirige** al usuario a la página de administración de productos, **mostrando** un mensaje de confirmación.

Flujo Alternativo (FA01): Cancelar operación 4.1. El usuario **decide** cancelar la modificación del producto. 4.2. El usuario **da clic** en el botón "Cancelar". 4.3. El sistema **redirige** al usuario a la página de administración de productos sin realizar ningún cambio.

Excepciones: EXC1: No hubo conexión a la base de datos al modificar el producto 5.1. El sistema **no puede** actualizar el producto en la tabla de productos debido a un error. 5.2. El sistema **muestra** un mensaje de error al usuario. 5.3. El usuario **se encuentra** en la página de edición de producto.

EXC2: Datos inválidos o faltantes 5.4. El usuario **ingresa** datos inválidos o falta información requerida. 5.5. El sistema **muestra** un mensaje de error y **solicita** al usuario que corrija los datos antes de continuar. 5.6. El usuario **permanece** en la página de edición de producto hasta que corrija los datos.

----

1. El sistema **muestra** la página de administración de pedidos con la lista de pedidos pendientes de validación.
2. El administrador **selecciona** un pedido de la lista.
3. El sistema **muestra** los detalles del pedido 
4. El administrador **revisa** la información del pedido.
5. Si la información es correcta, el administrador **aprueba** el pedido.
6. El sistema **cambia** el estado del pedido a "Aprobado" o "Rechazado" y **envía** una notificación al cliente por medio electronico
7. El sistema **muestra** un mensaje de confirmación al administrador.

Flujo Alternativo 1 (FA01): Rechazar pedido 5.1. Si la información del pedido es incorrecta o incompleta, el administrador **rechaza** el pedido. 5.2. El sistema **solicita** al administrador un motivo para rechazar el pedido. 5.3. El administrador **ingresa** el motivo de rechazo. 5.4. El sistema **cambia** el estado del pedido a "Rechazado" y **envía** una notificación al cliente con el motivo de rechazo. 5.5. El sistema **muestra** un mensaje de confirmación al administrador.


Excepciones: EXC1: Error al cambiar el estado del pedido 
6.1. El sistema **no puede** cambiar el estado del pedido debido a un error. 
6.2. El sistema **muestra** un mensaje de error al administrador. 
6.3. El administrador **tiene** la opción de **intentar** nuevamente

EXC2: Error al enviar la notificación al cliente 6.4. 
El sistema **no puede** enviar la notificación al cliente debido a un error. 
6.5. El sistema **muestra** un mensaje de error al administrador. 
6.6. El administrador **puede** **intentar** nuevamente o **continuar** con el siguiente pedido.