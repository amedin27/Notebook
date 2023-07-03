# 7- Contenedores y orquestación:
Doker desarrolló en 2009 e introdujo el concepto de los contenedores. 

## 7.1 ¿Qué son los contenedores?:
El concepto de contenedor viene del concepto de contenedor marítimo que se traslada a través de los cargueros. Estos contenedores dentro tienen diferentes mercancías. Para poder organozar el espacio y el transporte antiguamente se hacía muy difícil hasta que se introdujeron estos contenedores. Este concepto se traslada al mundo del desarrollo de la siguiente manera: 

Imagina que yo estoy trabajando con Windows 18 entonces yo voy a generar una app y la voy a testear y desplegar en mi propia máquina. En mi máquina funciona perfectamente. Pero ahora le pasamos el software a un amigo y lo intenta ejecutar, en ese momento salta un error y no lo puede ejecutar porque mi amigo tiene una versión anterior. Eso pasa porque las librerías y las dependencias que él tiene son incompatibles. Es aquí donde empieza a entrar el cocepto de contenedor. 

Antiguamente cuando yo quería alojar una app tenía que desarrollar mi alojamoento para que tuviera una infrastructura y crear una máquina virtual con el sistema operativo que yo quisiera. Después, necesitaba instalar todas las librerías para que pueda correr. Aquí es cuando entra en juego el concepto de contenedor. 

El contenedor tiene ya un encapsulamiento de el código fuente, las librerías y las despendencias y le pasamos las instrucciones del sistema operativo que tiene que utilizar. De esta manera nosotros estaríamos generando un contenedor que se puede ejecutar en cualquier lado. Una vez que yo ya tengo creado este contenedor , se lo puedo pasar a mi amigo que gracias a un "traductor" (Container engine) podría interpretar esto. Una de las ventajas que nos hace utilizar esto es que nos ahorra casi un 90% de recursos. 

Hoy en día hay diferentes tipos de contenedores: 
- Docker: Docker es una plataforma de virtualización de contenedores que permite empaquetar y distribuir aplicaciones junto con todas sus dependencias en un entorno aislado y autónomo llamado contenedor. Los contenedores de Docker son livianos, portátiles y escalables, lo que los hace ideales para desarrollar, implementar y ejecutar aplicaciones de manera consistente en diferentes entornos, ya sea en una computadora local, en servidores físicos o en la nube.
- Podman: Es un sistema muy similar a Docker pero con mejoras de rendimiento. 

## 7.2- ¿Qué es la orquestación?:
Imagina que tu como desarrollador, desarrollamos una interfaz que necesita tener acceso a un servicio de Back-End. El Front se conectaría con el Back para hacer unas operaciones. Por otro lado, también necesitaríamos la base de datos. 

El rol del desarrollador sería hacer un contendor para el Front otro para el Back y otro para la base de datos. Ahora lo que necesitamos es que estos contenedores se relacionen y tengan acceso a internet para que todo el mundo tenga acceso a ellos. Aquí es donde entra el concepto de lo que se conoce como "Master". 

La orquestación en el contexto de Docker se refiere a la capacidad de gestionar y coordinar múltiples contenedores de Docker como parte de una aplicación o servicio más grande. La orquestación permite administrar de manera eficiente y automatizada la creación, escalado, distribución, monitoreo y el mantenimiento de los contenedores en un entorno de producción. (Nodo)

Existen varias herramientas populares de orquestación en el ecosistema de Docker, como Docker Swarm, Kubernetes y Apache Mesos. Estas herramientas proporcionan funcionalidades para coordinar y administrar clústeres de contenedores, lo que simplifica el despliegue y la gestión de aplicaciones complejas y de alto rendimiento.
