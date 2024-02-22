Validar pedido

El administrador se encuentra en la *administración del pedido* y **visualiza los pedidos pendientes por validar** y cuando **selecciona uno se le muestra** *aceptar pedido*, donde se encuentran los detalles del pedido, el estado y los botones de confirmación. El administrador seleccionara aceptar y el **sistema cambiara el estado del pedido** en la *tabla de pedidos*, **notificara al cliente por correo** y **muestra al administrador un mensaje de afirmación**.

1. El sistema se muestra la pantalla de administración de pedidos
2. El administrador selecciona un pedidos
3. El sistema muestra la pantalla aceptar pedido donde se encuentran, los detalles del pedido, el estado y los botones de confirmación.
4. El administrador da click en el botón aceptar
5. El sistema guarda el nuevo estado del pedido en tabla del , envía un correo al cliente del pedido y muestra un mensaje de afirmación

Flujo alterno:

FA01:El administrador selecciona la opción rechazar en la pantalla aceptar pedido
	4.1 El administrador da click en el botón de rechazar
	5.1 El sistema mostrara un formulario para ingresar datos necesarios para el rechazo del pedido
	6.1 El administrador llenara el formulario con los datos y da click en boton enviar.
	7.1 El sistema cambiara el estado del pedido, envia un correo al cliente y muestra un mensaje de afirmacion.

Exec