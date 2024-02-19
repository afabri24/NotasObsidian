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



