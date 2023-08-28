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