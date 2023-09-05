SOA=Aplicacion orientada a servicios: es una arquitectura 

sistema multicapa
multinivel
multicanal

1.Consumiendo Servicio en aplicaciones Desktop
*Manejo de GUI de Java*
	 -Creacion de UI
	 -Manejo de Controles Basicos
	 -Manejo de Controles de Accesos a Datos
Necesito:
	-JDK 8
	-JavaFX
	-NetBeans(recomendacion 14)
	-Scene Builder
Sigue siendo la parte 1:
	-Servicios SOA/RESTful sobre la Tecnologia Java
	-Referencia a servicio SOA/RESTful
	-Creacion del Cliente de Servicio
	-Manipular datos con el Servicio SOA/RESTful

1.Consumiendo Servicios SOA/RESTful en Aplicaciones Desktop
	-Manejo de GUI en -Net con windows Presentation Fundation
	-Creacion de Windows WPF
	-Manejo de Contrioles Basicos
	-Manejo de Controles de Acceso a Datos
	-Binding 
2.Consumiendo Servicios SOA/RESTful en Aplicaciones Web
	 -Apliciones Web bajo de la Tecnologia Java
	 -Creando paginas Web
	 -Accediendo al Servicio SOA/RESTful
	 -Manipular Datos mediante el servicio SOA/RESTful
3.Consumiendo Servicios en Aplicaciones Para Dispositivos Moviles
	-Creacion de Apps para diapositivos Android
	-Creacion de Apps para dispositivos iOS


| Criterio de Evaluacion | Puntaje |
| ---------------------- | ------- |
| Examen                 | 30      |
| Tareas                 | 10      |
| Actividades            | 20      |
| Proyecto               | 40      |

---
#Introduccion

La *Computación Orientada a Servicios* es un paradigma de desarrollo que posibilita la construcción y ejecución de aplicaciones de usuario en ambientes distribuidos heterogéneos mediante la composición y el ensamblado de funcionalidad existente o servicio

Este paradigma tiene como prioridad el reúso y la interoperabilidad de las aplicaciones y servicios

Es el armazón sobre el que se construyen las comunicaciones entre distintos servicios. Su papel es critico para permitir, no solo su interacción , si no también su efectividad, haciendo posible con el fin que fue creados

Lo que es clave de estos servicios es su naturaleza desacoplada; la interfaz de servicios es independiente de la implementación

Un servicio es una funcionalidad concreta que puede ser descubierta de la red y describe tanto lo que puede hacer como el modo de interactuar con ella

Los servicio también pueden acoplarse dentro un a aplicación completa que proporcione servicios de alto nivel, con un grado de complejidad muy superior

La estrategia de orientación a servicios permite la creación de servicios y aplicaciones compuestas que pueden existir con independencia de las tecnologías adyacente


[![Arquitectura Orientada a Servicios (SOA) | Ingeniería del Software UAH](https://ingenieriadelsoftwareuah2015.files.wordpress.com/2015/03/soa-11.jpg)

A la hora de desarrollar, en lugar de crear aplicaciones enormes y muy complejas, se desarrollan componentes reutilizables que son fáciles de mantener y probar

[[Diferencia de Asincrono y sincrono]]

Esta arquitectura basada en servicios requiere una infraestructura de comunicaciones escalable y segura entre los componentes que se convierte en el eje vertebrado de todos los sistemas de la organización y que se conoce como *Enterprise Service Bus o Bus empresarial


soa: LLamada orientadas a servicios

Para SOA es indeferente la tecnologia que utilicemos, sin embargo, la tecnologia de Web Services o servicios Web es una de las que mas notoriedad ha conseguido.

Beneficios
	-Eficiencia
	-Capacidad
	-Adaptabilidad

#IntegracionSolucionesClase28/08/23

Servicios web:
Es una tecnologia que utiliza un conjunto de protocolos y estandares que sirven para intercambiar datos entre aplicaciones

Un servicio Web o WebService es un servicio ofrecido por una aplicación que expone su lógica a clientes de cualquier plataforma mediante una interfaz accesible a través de la red utilizando tecnologías(protocolos) estándar de internet
	-Se encuentra disponible a través de internet o una intranet
	-Usa una forma estandarizada de mensajería(generalmente XML)
	-No se encuentra atado a ningún sistema operativo ni ningún lenguaje de programación
	-Se puede auto describir (generalmente via XML)
	-Puede ser descubierto a traves de un mecanismo de busqueda

The organization for the Advacent of Structured Information Standards (OASIS) y el World Wide Web Consortium(W3C) son los responsables de la estandarizacion y arquitectura de los servicios web

La industria en su interés por el desarrollo de los servicios web ha creado la WS-I (Web Services Interoperability Organization) cuya Intención es la integración de los estándares que garanticen y mejoren la interoperabilidad de los servicios web

Al conjunto de servicios y protocolos para servicios webs conocido comúnmente como "Web Services Protocol Stack" y básicamente son utilizados para definir, localizar, implementar y hacer que un servicio web interactúe con otro

Este conjunto esta conformado esencialmente de cuatro conjuntos:
	-Servicio de transporte
	-Mensajería XML
	-Descripción de servicio
	-Descubrimiento de Servicios

**Servicio de transporte:**
Es el encargado del trasporte de los mensajes entre aplicaciones sobre la red. incluye protocolos del nivel de aplicación. A continuación se relata  sobre los mas utilizados
	-http(HyperText Transfer Protocol):
		Protocolo del nivel de aplicación mas utilizado en la internet. es el protocolo que define la sintaxis y la semántica utilizada para la arquitectura web. En el contexto de los servicios web es utilizado par ala transferencia de transacciones XML a través de la red utilizando los mismos principios del HTML
	-FTP(File Transfer Protocol):
		Es un protocolo de la capa de aplicación encargado de los servicios de transmisión de archivos a través de redes soportadas sobre TCP. En el ámbito de los servicios web el FTP
		permite realizar modificaciones remotos evitando el uso de permisos
	SMTP(Simple  Mail Transfer Protocol):
		Es un estándar de la capa de aplicación ampliamente utilizado para el envió de mensajes de coreo electrónico a través de internet. Es un estándar de Facto basado en texto, que requiere como cliente software de tipo POP3 o IMAP


**Mensajeria XML:**
	Es el conjunto encargado de la codificación de los mensajes XML y pueda asi ser interpretado en cualquiera de los nodos de la red. los componentes mas utilizados en este conjunto son los siguientes
		-REST(reprensentational State Transfer):
			Fieldieng da la siguiente definicion: "estilo de arquitectura de software para sistemas hiper medias distribuidos tales como la World Wide Web". En resumen es un conjunto de principios para diseño de redes, que es utilizado comunmente para definir una interfaz de transmision HTTP de manera analoga como lo hace SOAP
		RPC(Remote Procedure Calls):
			Es una tecnologua de software que permite ejecutar una rutina en un equipo o segmento de red de manera remota.
		XML(eXtended Markup Language):
			XML es uno de los lenguajes mas utilizados para el intercambio de datos sobre la web. Su desarrollo se remota en el año 1996 por el grupo de trabajo de la Word Wide Web Consortium lanzado su primera version el 10 de Febrero de 1998

Descripcion del Servicio:
 El servicio web debecontar con una interfaz publica la cual es descrita por un formato llamado WSDL (Web Services Description Language)
	 WSDL:
	 es un tupo de un documento XML que describe lo que hace un servicio web, donde se encuentra la forma de ser invocado.
	 Este provee informacion muy importante para los desarrolladores, este lenguaje describe el formato de los mensajes que utiliza y las cuales puede responder.
		 Tipos
			 Tipos de datos usados por los mensajes
		 -Mensaje:
			 Que datos son enviados desde un nodo a otro
		 Limite:
			 Es la descripción del protocolo que se esta utilizando para transportar el mensaje que puede ser HTTP, Post, HTTP, GET, SOAP y MIME

#IntegracionSolucionesClase29/08/23

Estilo Arquitectonico REST
REST(Representational State Transfer) es una forma ligera de crear servicios web
El elemento principal en el que se basan estos servicios son las URLs. En general podemos decir que estos servicios consisten en URLs a las que podemos acceder, por ejemplo mediante el protocolo HTTP, para obtener información o realizar una operación

El formato de la informacion que se intercambie con estas URLs lo decidira el desarrollador del servicio

Este tipo de servicios acercan los Servicios Web al tipo de aquitectura de la web, siendo especialmente interesantes para utilizacion en AJAX

Debe ser un sistema cliente-servidor

Tiene que ser sin estado, es decir no hay nacesidad de que los servicios guarden las sesiones de los usuarios(cada peticion al servicio tiene que ser independinte de las demas)

Debe soportar un sistema de caches: la infraestructura de la red debería soportar cache en diferentes niveles

Debe ser un sistema uniformente accesible( con una interfaz uniforme): cada recurso debe tener una unica direccion y un punto valido de acceso. Los recursos se identifican con URIs, lo cual proporciona un espacio de direccionamiento global para el descubrimiento del servicio y de los recursos


Tiene que ser un sistema por capas: por lo tanto debe soportar escalibilidad

Debe utilizar mensajes auto-descriptivos: los recursos se desacoplan de sus represntacion de forma que puedan ser accedidos en una variedad de formatos, como por ejemplo XML,HTML,Textoplano,PDF,JPEG,JSON,etc.

A continuacion se explicaban las abstracciones que constituyen un sistema RESTful:
Recursos
Representacionciones
URIs
Tipos de peticiones HTTP que constituyen la interfaz uniforme

Un recurso REST es cualquier cosa que sea direccionable a través de la web
por direccionable nos referimos a recursos que puedan ser accedidos y transferidos entre clientes y servidores

Por lo tanto, un recurso es una correspondencia lógica y temporal con un concepto en el dominio del problema para el cual estamos implementado una solución

Algunos ejemplos de recursos REST son:
	Una noticia de un periódico
	la temperatura de Xalapa a las 4:00 pm
	un valor de IVA almacenado en una base de datos
	una lista con el historial de las asistencias en un sistema empresarial

Aun cuando el mapeado de un recurso es único, diferentes peticiones a un recurso pueden devolver la misma representación binaria almacenada en el servidor

Debido a que estamos utilizando HTTP para comunicarnos, podemos transferir cualquier tipo de información que pueda trasportarse entre clientes y servidores

Los datos de WS son transferidos TCP/IP y el navegador conoce como representar los streams binarios debido a la cabecera de respuesta del protocolo HTTP Content-Type

Por lo tanto, en un sistema RESTful, la representación de un recurso depende del tipo deseado por el cliente(tipo MIME), el cual esta especificado en la petición del protocolo de comunicaciones

la representacion de los recursos es lo que se envia entre los servidores y clientes

Una representacion muestra el estado del dato real almacenado en algun dispositivo de almacenamiento en momento de la peticion

En terminos generales es un stream binario, juntamente con los metadartos que describen como dicho stream debe ser consumido por el cliente y/o servidor(los metadatos tambien pueden contener informacion extra el recurso, como por ejemplo informacion de validacion y encriptacion, o codigo extra para ser ejecutado dinamicamente)

A traves del ciclo de vida de un servicio web, pueden haber varios clientes solicitando recursos
Clientes direntes son capaces de consumir diferentes representaciones del mismo recurso . por lo tanto la representacion puede tener varias formas como por ejemplo una imagen, un texto, un fichero XML, o un fichero JSON, pero tienen que estar disponibles en la misma URL

El lenguaje para intercambio de informacion con el servicio queda a eleccion del desarrollador

A acontinuacion se muestran formatos comunes que podemos utilizar par aintercambiar esta informacion:

| formato     | tipo MIME      |
| ----------- | -------------- |
| Texto plano | text/plain     |
| html        | text/html      |
| xml         | aplication/xml |

Una URI o Uniform Resorce Indentifieer es un servicio web RESTful es un hiper-enlace a un recurso y es la unica forma de intercambiar respresentaciones entre clientes y serdores

Un servicio web RESTful expone un conjunto de recursos que indentifican los objetivos de la interacioncon sus clientes

En un sistema REST, la URI no cambia a lo largo del tiempo ya que la implementacion de la aquitectura es la que gestiona los servicios localiza los recursos, negocia las representaciones y envian respuestas con los recursos solicitados

y lo que es mas importante, si hubiese un cambio en la estructura del dispositivo de almacenamiento en el lado del servidor( por ejemplo, un cambio de servidores de bases de datos), nuestras URIs seguiran siendo las mismas y seran validas mientras el servicio web siga estando " en marcha" o el contexto del recurso no cambie

Sin las restricion REST, los recursos se acceden por su localizacion: las direcciones web tipicas son URIs fijas. Si por ejemplo renombramos un fichero en el servidor, la uri sera diferente; si movemos a un directorio diferente la URI tambien sera diferente.

por ejemplo, si en nuestra aplicacion tenemos informacion de cursos podriamos acceder a la lista cursos que el desarrollador del sevicio haya decidido

peticiones HTTP
en su forma mas simple, los servicios web RESTful son aplicaciones xliente-servidor a traves de la red que manipulan el estado de los recursos

en este contexto, la manipulacion de rexuros significa creacion de recursos, recuperacion, modificaciony borrados.(Create, Retrieve, Update, Delate[CRUD])

Sin embargo, los sercicios web RESTful no estan limitados solamente a estos conceptos basicos de manipulacion de  datos

por el contrario los servicios RESTful pueden ejecutar logica en al lado del servidor, pero recordando que cada respuesta debe ser una representacion del recuros del dominio en cuestion

debemos determinar que operacion HTTP se ajustamejor a la manipulacion que desamos realizar sobre los datos

| Accion sobre los datos | Protocolo HTTP equivalente |
| ---------------------- | -------------------------- |
| CREATE                 | POST                       |
| RETRIEVE               | GET                        |
| UPDATE                 | PUT                        |
| DELETE                 | DELETE                           |

GET 

El metodo GET se utiliza para recuperar recursos

El metodo HTTP GET solamente deberia utilizarse para recuperar representaciones. Podriamos utilizar una peticion GET para actualizar el estado de los datos en el servidor pero no es recomendable

los parametros de este metodo se envian sobre la URI del recurso

Una operacion debe ser segura e idempodente

Idempodente: es la propiedad para realizar una accion determinada varias veces y aun asi conseguir el mismo resultado se obtendria si se realizase una sola vez

Estos servicios pueden ser probados directamente sobre el navegador

POST/CREATE

El metdodo POST se utiliza para crear recursos

Las peticiones POST no son idempotentes

los parametros de este metodo se envian del cuerpo del mensaje

Estos servicios NO pueden ser probados directamente sobre el navegador

PUT/UPDATE

El metodo PUT se utiliza Actualizar(modifcar)recursos o para crearlos si el recuros en la URI especificada no existiese previamente

Es decir, PUT se utiliza para establecer un determinado recursos dada su URI

A diferencia de POST, Pur es idempotente

DELETE

El metodo DElete se utiliza para BORRAR representaciones

los para metros de este metodo se envian sobre el cuerpo del mensaje

Estos servicios NO pueden ser probados directamente sobre el navegador


Entity:
conexion a base de datos y manipulacion de datos
mapea