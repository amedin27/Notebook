## 4.8 Bases de datos:
Una base de datos es un sistema organizado de almacenamiento y gestión de información estructurada. Consiste en una colección de datos interrelacionados que se almacenan en un formato específico y se gestionan mediante software de base de datos.

Las bases de datos se utilizan para almacenar, organizar y recuperar información de manera eficiente. Proporcionan una estructura y un conjunto de reglas que permiten almacenar grandes cantidades de datos de forma sistemática y coherente. Esto facilita el acceso y la manipulación de los datos, así como la realización de consultas y análisis.


### 4.8.1 Fases en el proceso de creación de bases de datos:
En general, el proceso de creación de una base de datos puede dividirse en varias fases. A continuación, se describen las fases típicas en el desarrollo de una base de datos:

Análisis de requisitos: En esta fase inicial, se identifican y analizan los requisitos y las necesidades de la base de datos. Se trabajará en estrecha colaboración con los usuarios finales y los interesados para comprender los datos que se deben almacenar, las relaciones entre ellos, los informes requeridos y otras funcionalidades necesarias.

Diseño conceptual: En esta etapa, se crea un diseño conceptual de la base de datos. Se definen las entidades, los atributos y las relaciones clave. Se utilizan herramientas como diagramas de entidad-relación (ER) para visualizar la estructura de la base de datos de manera clara.

Diseño lógico: En esta fase, se realiza la traducción del diseño conceptual en un modelo lógico de la base de datos. Se utilizan modelos de datos específicos, como el modelo relacional, para definir las tablas, los campos y las restricciones de integridad. También se definen las claves primarias y las relaciones entre las tablas.

Diseño físico: En esta etapa, se realiza la implementación concreta de la base de datos. Se definen los tipos de datos específicos, los índices, las particiones y otros detalles técnicos. También se determina cómo se almacenarán y se organizarán los datos en los dispositivos de almacenamiento físico.

Implementación y carga de datos: En esta fase, se crea la estructura de la base de datos y se cargan los datos iniciales. Se utilizan lenguajes y herramientas específicas, como SQL, para crear las tablas, los índices y otras estructuras necesarias. Luego, se realiza la carga inicial de datos en la base de datos.

Pruebas y verificación: Una vez que la base de datos está implementada y los datos están cargados, se realizan pruebas exhaustivas para verificar la integridad, la precisión y el rendimiento de la base de datos. Se comprueba que las consultas, los informes y otras operaciones funcionen correctamente.

Despliegue y mantenimiento: Una vez que la base de datos ha pasado por todas las fases anteriores y se ha verificado su funcionamiento, se despliega y se pone en producción. A partir de ese momento, se realiza el mantenimiento continuo de la base de datos, lo que implica realizar copias de seguridad, aplicar actualizaciones y optimizar el rendimiento a medida que sea necesario.

### 4.8.2 Tipos de bases de datos:
- Bases de datos SQL: Una base de datos SQL (Structured Query Language) es un tipo de base de datos que utiliza el lenguaje de consulta estructurado (SQL) para gestionar y manipular datos. SQL es un lenguaje estándar utilizado para la comunicación con las bases de datos relacionales. Se le conoce también como bases de datos relacionales.

En una base de datos SQL / relacionales:, los datos se almacenan en tablas que están organizadas en filas y columnas. Las tablas están relacionadas entre sí mediante claves primarias y claves foráneas.
- Bases de datos no SQL:Las bases de datos NoSQL (Not Only SQL) son un tipo de bases de datos que difieren de las bases de datos SQL en su modelo de almacenamiento y recuperación de datos. A diferencia de las bases de datos SQL, las bases de datos NoSQL no utilizan el lenguaje de consulta estructurado (SQL) como su principal medio de manipulación de datos.

Las bases de datos NoSQL / no relacionales: se han desarrollado para abordar desafíos específicos en la gestión de grandes volúmenes de datos no estructurados, como datos de redes sociales, registros web, datos de sensores y otros tipos de información no tabular. Estas bases de datos se caracterizan por su capacidad para escalar horizontalmente y gestionar grandes cantidades de datos distribuidos en múltiples .servidores. También conocidas como bases de datos no relacionales.

| Tipo de Base de Datos | Ejemplos Relacionales    | Ejemplos No Relacionales |
|-----------------------|--------------------------|--------------------------|
| Relacionales          | MySQL, PostgreSQL, Oracle| -                        |
| Documentos            | -                        | MongoDB, Couchbase, Firebase|
| Clave-Valor           | -                        | Redis, Riak, Apache Cassandra |
| Columnas              | -                        | Apache HBase, ScyllaDB, Amazon DynamoDB |

