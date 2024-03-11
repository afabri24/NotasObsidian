## Datos del maestro

Miguel Angel Ortigaza Clemente

Lic. informatica -> FEI UV  2015

Mtr -> UFM 2020

mortigoza@uv.mx

Eminus 4 y Teams

Clases 2017 - Actualidad
## Programa

### Temas

- Introducción alas bases de datos  NoSQL
- Manejo de grandes cantidades de datos 
	- Modelo de documentos 
	- modelo clave-valor
	- Modelo de columnas
	- Bases de datos de grafos
- Modelos de distribución
	- Servidor ...

Evaluacion:

| Material            | Porcentajes |
| ------------------- | ----------- |
| Examen teorico      | 15          | 
| Examen practico     | 15          |
| Practicas           | 40          |
| Proyecto integrador | 30          |
# Introducción a las bases de datos no convencionales


###### ¿Qué es una base de datos?

Una base de datos es una recopilación organizada de información o datos estructurados , que normalmente se almacena de forma electrónica en un sistema informático. Normalmente, una base de datos esta controlada por un sistema de gestión de bases de datos.

###### AAA

Autentificacion
Autorizacion
Accounting


Las bases de datos son el producto de la necesidad humana de almacenar la informacion,  es decir, de preservarla contra el tiempo y el deterior, para poder acudir a aella posteriormente. En ese sentido indispensable para almacenar enormes cantidades de datos en espacios fissicos limitados.

El manejo de las bases de datos se lleva mediante sistemas de gestión ( llamados DBMS Por sus siglas en ingles: Database Management Systems o sistemas de gestión de datos), que permiten el almacenamiento ordenado  y la rápida recuperación de la información.


En la conformación de una base de datos se pueden seguir diferentes modelos y paradigmas, cada uno dotado de características, ventajas y dificultades, haciendo énfasis en su estructura organización al, su jerarquía, su capacidad de de trasmisión o de interrelación, etc. esto se conoce como modelos de base datos y permite el diseño y la implementación de algoritmos y otros mecanismos de gestión según sea el caso especifico.


## Modelo de base de datos relacionales

Es un tipo de base de datos que almacena y proporciona acceso a puntos de datos relacionados entre si. Se basan en el modelo relacional, una forma intuitiva y directa de representar datos  en tablas. Normalmente utilizan un lenguaje de consulta estructurada (SQL) para escribir y consultar datos.


## Bases de Datos NoSQL

Una base de datos NoSql, o base de datos no relacional, permite almacenar y manipular datos no estructurados y semiestructurados( a diferencia de una base datos relacional, que define como se deben componer todos los datos insertados en la base de datos)

NoSql, clave-Valor, Documentales, grafos
[[Drawing 2024-02-15 16.34.06.excalidraw]]

### Modelo clave valor
Destacan por se muy eficientes tanto como la lectura como para escritura. Cada elemento esta identificado por una clave única que permite recuperar datos rápidamente. Los datos suelen estar almacenados como objetos binarios.

### Modelo orientado a documentos
son las bases de datos NoSQL mas versatiles y que se pueden usar en una gama amplia de proyectos. Permiten realizar consultas mas avanzadas sobre el contenido de un documento, además de consultas de clave- valor. Se apoyan simples como JSON o xml

### Modelo orientadas a grafos
Ofrecen una experiencia de búsqueda mas eficiente entre relaciones, respecto a las bases de datos relacionales. Este modelo usa estructuras de grafos para consultas semánticas y representa los datos como nodos, bordes y propiedades


### Modelo orientada a objetos
Agrupa la información en paquetes relacionados entre si: Los datos de cada registro  se combinan en un solo objeto, con todos sus atributos. De esta manera, toda la información esta disponible en el objeto, ya que sus datos quedan agrupados en el lugar de distribuidos en diferentes tablas.
En los objetos no solo pueden guardarse los atributos, sino también los métodos que refleja la afinidad de estas bases de datos con los lenguajes de programación orientada a objetos: Al igual que en estos, cada objeto representa un conjunto de acciones que pueden llevarse a cabo.

Se basa en el concepto de encapsular elementos de datos, sus características, atributos y el código que opera sobre en elementos complejos llamados objetos.


## Bases de Datos Distribuidas

Una base de datos distribuida consta de dos o mas archivos que se encuentran en sitios diferentes. La base de 
datos puede almacenarse en varios ordenadores, ubicarse en la misma física o repartirse en diferentes redes.


# Bases de de datos NoSQL

NoSQL se refiere a una base de datos no relacional o no sql
NoSQL significa " Not only SQL" y es asi hay que entender el modelo de bases de  datos: no se trata del elemento antagónico, sino de un enriquecimiento y complemento útil de las tradicionales bases de datos relacionales

las aplicaciones modernas usan y generan tipos de datos complejos y que cambian constantemente, y las bases de datos relaciones no fueron diseñadas para gestionar este tipo de almacenamiento y recuperación de datos. Las bases de datos NoSQL son mas flexibles y escalables.

El desarrollo de las bases de datos NoSQL, que surgió en respuesta a las limitaciones y los problemas de las bases de datos relacionales, supuso la creación de una autentica alternativa, ya que en muchas ocasiones las bases de datos relacionales ya no son capaces de hacer frente a las exigencias del desarrollo moderno de aplicaciones


## Bases de datos Documentales

Se utilizan para la administración de datos semiestructurados. Se trata de datos que no siguen una estructura fija, sino que llevan la estructura casi en si misma. Sin embargo, con ayuda de marcadores dentro datos, la información pueden ordenarse.

Crea un par simple: un documento especifico se asigna a una clave. En este documento, que puede tener formato XML, JSON o YAML, por ejemplo, se puede encontrar las información propiamente dicha. Como la base de datos no requiere un esquema especifico, en un almacén de documentos pueden integrarse diferentes clases de documentos. los cambios de documentos no cambian la base de datos.

	BaseX: Este proyecto open source utiliza Java y XML. Base X viene con una interfaz de usuario.
	MongoDB: MongoDB es la base de datos NoSQL mas extendida del mundo. El software esta escrito en c++ y emplea similares a JSON
	simple DB:

## Bases de datos de grafos

Es un conjunto s de objetos(Vertices y aristas) que permite representar datos interconectados, asi como las relaciones entre ellas, de forma comprensible y como un unico y mas amplio conjunto de datos.

Un ejemplo tipico del uso de bases de datos de grafos es el analisis de las relaciones entre los usuarios de las redes sociales o de los habitos de compra de los clientes en tiendas online.

Recomendaciones personalizadas de compra o de amistades
Crear perfiles completos de clientes
Analisis de riesgo
Deteccion de fraudes
Busqueda de errores


	Neo4j: Neo4j es la graph database mas poular y esta concebida como modelo de codigo abiertom
	amazon neptum:
	Sap hana Graph:
	OrientDB:

## Bases de datos de clave-valor
Esta modalidad de base de datos, basa en una tabla de tan solo dos columnas, en una de ellas se guarda valor y en una en la otra que representa una cacteristica identificativa unica.

Redis

amazon DynamoDB:
Berkeley DB
Voldermolt


Tecnologias que vamos a utilizar:
BaseX->XML
MongoDB->JSON
NEO4j
Redis

## Base de datos columnar

Mientras que la mayoria de las bases de datos distribuyen la informacion en filas, las bases de datos columnares funcionan de la manera contraria: se distrubuyen en columnas

amazon redshift
mariaDB-columnStore:
sap HANA
Apache cassandra
monetDB


# ¿Por que usar una base de datos NoSQL?
Mejor rendimiento
Permite resolver problemas con el escalado de grandes volúmenes de datos relacionales
estructurados, a la vez que hace posible la latencia baja y un rendimiento alto.
Mejores datos
Mas flexibilidad para utilizar cantidades masivas de datos estructurados, semi estructurados y no estructurados, así como datos relacionales.


Costos reducidos

Velocidad de llegada al mercado


# Bases de datos SQL

## LDD
Lenguaje de definición de datos(LDD)
El LDD de SQL proporciona ordenes para la creación, modificación y eliminación de base de datos y tablas(esquemas de relación), a su vez permite la creación de índices, llaves primarias y foráneas.

También incluye ordenes para la definición de vistas, funciones y procedimientos almacenados de base de datos.

## LMD
El LMD de SQL es un lenguaje orientado a consultas, esta basado tanto en el algebra relacional como en el calculo relacional de tuplas.
incluye ordenes para consultar, insertar, modificar y borrar filas(tuplas) de las tablas de la base de datos.

## Algebra relacional

El algebra relacional es un lenguaje de consulta procedimental.

Todas las operaciones de álgebra relacional SIEMPRE tienen como resultado una tabla temporal


Reunión externa 

La reunión externa es utilizada cuando se requiere conservar las filas de una tabla al reunirla con otra a apesar que no cumplan con las condiciones especificadas.

Los 2 principales tipos de reunión externa:

Reunión externa derecha
Reunión externa izquierda


La relacion/tabla objetivo sera la que se encuentra a la izquierda de la operacion, el resultados seran todas las tuplas en relacion de la izquierda

debian



avg
min
max
sum
count


Group by



SELECT G1,G2..GN,F1(A1),F2(A2),...,Fn(AN) FORM R GROUP BYE G1,G2..GN

R. es la relacion o tabla
G. Es el nombre del atributo AGRUPADOR
F. Es una funcion de agregacion
A. Es un nombre de atributo que se va agregar.


Select nombre, AVG(calificacion) AS promedio FROM ALUMNO GROUP BY nombre



sql
1. Primero se ejecutan las operaciones de producto cartesiano, Reunion o Reunion Externa.
2. Despues se aplican los predicados o condiciones de la operacion seleccion (WHERE).
3. se aplican las agrupaciones(GROUP BY)
4. Se aplica la proyeccion de las columnas
5. Se realizan los ordenamientos de datos

() = subconsulta



# Modelo de datos

Los modelos de datos desempeñan una funcion esencial a la hora de reunir a todos los segmentos de una empresa, es decir, a los de TI




Es el proceso de cracicion de una representacion visual o esquema que define los sistemas de recopilación y administacion de informacion de cualquier organización


El modelado de datps puede adoptar diferentes enfoques(conceptual, logico o fisico) y consiteen la realizadion de una serie de  tareas previas


- identificar tipos de entidades
- identificar atributos
- Aplicar convenciones de nomenclatura
- Identificar relaciones
- Aplicar modelos de modelos de datos
- asignar claves
- Normalizar para reducir la redundancia de datos
- Desnormalizar para mejorar el rendimiento


## Modelado conceptual de datos
Define la estructura general de su negocio y sus datos
Los modelos de datos conceptuales ofrecen un a visión global de los datos explican lo siguiente:

- ¿Que datos contiene el sistema?
- Atributos de los datos, asi como las condiciones o restricciones de los mismos
 - ¿Con que reglas empresariales se relación los datos?
- ¿Como se organizan mejor los datos?
- Requisitos de seguridad e integridad de datos

## Modelado lógico de datos
Una vez que el dominio del problema y los conceptos iniciales están mas claros gracias al modelado de datos conceptuales, es el momento de ser mas especifico con un modelo de datos lógicos


## Modelado físico de datos
Un modelado físico de datos en su implementación especifica del modelo lógico de datos, y lo crean los administradores de la base de datos y los desarrolladores




# Modelo Documental

Se utilizan para la administración de datos semiestructurados. Se trata que no siguen una estructura fija, sino que llevan la estructura casi en si misma. Sin embargo, con ayuda demarcadores dentro de estos datos, la información puede ordenarse


Las bases da datos de documentos permiten una indexación fácil, potentes consultas ad hoc y analisis de colecciones de documentos