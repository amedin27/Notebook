# 11. MVC Modelo Cliente Servidor
El modelo Cliente-Servidor (también conocido como Modelo Cliente-Servidor o Arquitectura Cliente-Servidor) es un paradigma de diseño ampliamente utilizado en el desarrollo de sistemas de software y aplicaciones distribuidas.

En este modelo, el sistema se divide en dos componentes principales:

- Cliente: Es el componente que solicita servicios o recursos al servidor. El cliente puede ser una aplicación, un dispositivo o una interfaz de usuario que interactúa directamente con los usuarios. Su función principal es enviar solicitudes al servidor y procesar las respuestas recibidas.

Servidor: Es el componente que recibe las solicitudes del cliente, procesa esas solicitudes y envía las respuestas correspondientes de vuelta al cliente. El servidor es responsable de gestionar los recursos, como bases de datos, archivos y servicios, para satisfacer las solicitudes de los clientes de manera eficiente y segura.

El modelo Cliente-Servidor se basa en la comunicación a través de una red, como Internet, donde el cliente y el servidor pueden estar ubicados en diferentes máquinas físicas. El cliente y el servidor se comunican utilizando protocolos de red estándar, como HTTP, TCP/IP o WebSocket.

El modelo Cliente-Servidor ofrece varias ventajas, como la capacidad de distribuir la carga de trabajo entre múltiples servidores, permitiendo escalabilidad y modularidad. Además, facilita la centralización y la administración de recursos compartidos, lo que simplifica el mantenimiento y la actualización del sistema.

# 11.1 Estructuras de cliente servidor por niveles.
- Estructuras de un solo nivel: Consiste en tenerlo todo en una sola máquina (cliente, servidor y bases de datos)
- Estructura en dos niveles: Tenemos el cliente y a través de internet tenemos almacenado en otra máquina el servidor y la base de datos. 
- Estructura de tres niveles: Tenemos una máquina con el cliente, otra con el servidor y otra con la base de datos. 
- Estructura de N niveles: El cliente a través de internet acede a N servidores alojados en otra máquina y la base de daris está(n) en otra máquina. 


# 11.2 Tipos de servidores.
- Servidores web: Los servidores web son programas o aplicaciones informáticas que ofrecen servicios de alojamiento y entrega de páginas web y otros recursos a través de Internet. Estos servidores son responsables de recibir solicitudes de los clientes (generalmente navegadores web) y enviarles las respuestas correspondientes.En términos más técnicos, un servidor web es un software que se ejecuta en un servidor físico o virtual y se comunica con los clientes utilizando protocolos de comunicación web, como HTTP (Hypertext Transfer Protocol) o HTTPS (HTTP Secure). Al recibir una solicitud HTTP de un cliente, el servidor web procesa la solicitud, busca y recupera los archivos solicitados, y luego los envía al cliente como respuesta.
  
- Servidores FTP:Los servidores FTP (File Transfer Protocol) son aplicaciones o servicios que permiten la transferencia de archivos entre sistemas remotos a través de Internet. FTP es un protocolo estándar de red utilizado para la transferencia de archivos y sigue un enfoque cliente-servidor similar al modelo Cliente-Servidor.El servidor FTP proporciona un almacenamiento centralizado de archivos y directorios, y los clientes FTP pueden conectarse a este servidor para acceder, subir, descargar, eliminar y administrar archivos y directorios en el servidor remoto.

- Servidores de e-mail: Los servidores de correo electrónico, también conocidos como servidores de e-mail o servidores SMTP/POP/IMAP, son sistemas que se encargan del envío, recepción y almacenamiento de correos electrónicos.
  
- Servidor VPN: Un servidor VPN (Virtual Private Network) es un servidor que proporciona una conexión segura y privada a través de una red pública, como Internet. El servidor VPN actúa como un intermediario entre el dispositivo del usuario y el resto de Internet, permitiendo que la comunicación se realice de forma cifrada y protegida.Cuando un usuario se conecta a un servidor VPN, su dispositivo establece un túnel seguro con el servidor a través del cual se envían y reciben los datos. Esto garantiza que la información transmitida esté encriptada y protegida contra posibles interceptaciones o accesos no autorizados.

- Servidores PROXY:Un servidor proxy es un intermediario entre un dispositivo de cliente (como un ordenador o un teléfono) y otros servidores en Internet. Actúa como un punto de acceso y gestiona las solicitudes de los clientes hacia los servidores de destino. Cuando un cliente realiza una solicitud a través de un servidor proxy, este reenvía la solicitud al servidor de destino en nombre del cliente. El servidor proxy puede realizar varias funciones, como el filtrado de contenido, la mejora del rendimiento, la ocultación de direcciones IP o el balanceo de carga.


# 11.3 Modelo P2P (Blockchain)
El modelo P2P (Peer-to-Peer, de igual a igual en español) es un paradigma de arquitectura de red en el que los dispositivos o nodos de una red se comunican directamente entre sí, sin la necesidad de un servidor centralizado. En un entorno P2P, todos los dispositivos son considerados iguales y pueden actuar tanto como clientes como servidores al mismo tiempo.

En lugar de depender de un servidor central para la gestión de recursos y la intermediación de comunicaciones, los nodos P2P se conectan y colaboran directamente entre sí. Esto permite compartir y distribuir recursos, como archivos, ancho de banda, servicios y aplicaciones, de manera descentralizada.