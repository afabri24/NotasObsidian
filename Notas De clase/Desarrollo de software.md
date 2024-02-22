# Medologia ICONIX
## Fases:
	- Analisis de requisitos
	- Analisis y diseño preliminar
	- Diseño
	- Imprementacion

## Carateristicas Generales:
 - Interactivo e incremental
 - Orientado a aobjetos
 - Participacion activa de skateholders
 - Adaptable a las necesidades
 - Guiada por casos de uso
 - NO SE CONTRUYE SOFTWARE HASTA TENER DISEÑO
 - Uso dinamico de UML
	 - Diagramas de secuencia
	 - Diagramas de casos de uso
- Trazabilidad(Cada paso esta refenciado por un requisito)

## Analisis de requisitos:
Formas de extraccion de requisitos
	 Formularios
	 entrevistas
	 Persona-Persona
	 Observacion y analisis
	 Formulario
	 Analisis de Situacion
Resultados de esta fase:
	Lista de requisitos funcionales y no funcionales

## Definicion de requirimientos:
-Necesidad
-Caracteristicas, funciones y restricion
		Ejemplo
			Caracteristicas{
			- El usuario requiere  onsultar su calificacion de IHC
			- El usuario debe poder iniciar sesion
			- El sistema debe buscar e indicar las existencias en la BD
			- El sistema debe estar disponible a traves de internet
			}
			Restricciones{
			- Solo estudiantes de la UV pueden entrar
			- El usuario solo puede ver sus calificaciones
			- El sistema solo puede buscar el producto
			- Siempre y cuando el usuario lo haga ingresado
			- Restricciones Tecnologicas
			- " De tiempo
			- Longitud de caracteres/contraseña
			}

## Requisitos
Requisitos que nos entrega el cliente:
Iniciar sesion
cerrar sesion
Conexion a BD en la nube



Requisitos que salieron a partir del analisis
Dar de alta paciente
registrar consulta
Registrar diagnostico



## Enfoque ICONIX

Modelado de objetos conducido por casos de uso
centrado en datos: se descompone en fronteras de datos
[[c0875248d1922e7c3e9933a3f91ac37b_MD5.jpeg|Open: images.jpeg]]
![[c0875248d1922e7c3e9933a3f91ac37b_MD5.jpeg]]

## Preguntas Iniciales

¿Quiénes son los usuarios (actores) del sistema y qué tratan de hacer?
¿Cuáles son los objetos del mundo real (dominio del problema) y las asociaciones entre ellos?¿Qué objetos son necesarios para cada caso de uso?
¿Cómo colaboran los objetos en cada caso de uso?
¿Cómo se manejan aspectos de tiempo real?
¿Cómo se construirá realmente el sistema a nivel de piezas?


Características
• Flexible para diferentes estilos y clases problemas.
• Apoyo a la manera de trabajo de la gente.
• Guía para los menos experimentados.
• Expone los productos anteriores al código de manera estándar y comprensible.


# Diagramas de robustez

Estas reglas ayudan a imponer un patron sustantivo-verbo-sustantivo en el texto de su caso de uso. Si el texto de su caso de uso sigue este patron, los diagramas de robustex son faciles de dibujar 