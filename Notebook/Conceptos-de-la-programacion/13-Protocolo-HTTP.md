# 13-Protocolo HTTP:
HTTP(Hypertext Transfer Protocol) : Cuando nació estaba concebido para tranmitir HTML pero evolucionó y ahora se tranfieren todo tipo de archivos. 

Es un protocolo de comunicación utilizado en internet para el intercambio de información entre un servidor y un cliente.Por ejemplo, imagina que el servidor es como una tienda online y el cliente eres tú, visitando esa tienda desde tu navegador web. Cuando solicitas algo a través de tu navegador, como abrir una página web o enviar un formulario, tu navegador utiliza el protocolo HTTP para comunicarse con el servidor y obtener la información que solicitas.

El funcionamiento básico del protocolo HTTP se basa en solicitudes y respuestas. Cuando tu navegador desea obtener una página web, envía una solicitud HTTP al servidor. Esta solicitud incluye información como el tipo de solicitud (por ejemplo, obtener o enviar datos), la dirección de la página web solicitada y otros datos adicionales.

El servidor recibe la solicitud y procesa la información. Luego, envía una respuesta HTTP de vuelta al cliente, que contiene la información solicitada. La respuesta puede incluir el código de estado para indicar si la solicitud fue exitosa (como el código 200 para "OK") o si hubo algún error.

Además de la solicitud y la respuesta, el protocolo HTTP también permite el intercambio de otros tipos de información, como encabezados HTTP. Estos encabezados proporcionan detalles adicionales sobre la solicitud o la respuesta, como el tipo de contenido que se está enviando o recibiendo.

Un protocolo es un conjunto de reglas estandarizadas para que diferentes tecnologías puedan comunicarse entre sí. 

## 13.1-Diferencia entre http y https:
La diferencia principal entre HTTP (Hypertext Transfer Protocol) y HTTPS (Hypertext Transfer Protocol Secure) es la capa de seguridad que proporciona HTTPS.

HTTP es el protocolo estándar utilizado para la comunicación entre un cliente (como un navegador web) y un servidor en internet. Sin embargo, HTTP no proporciona una capa de seguridad para proteger la información durante la transmisión. Esto significa que cualquier dato que se envíe a través de una conexión HTTP puede ser interceptado y leído por terceros.

Por otro lado, HTTPS es una versión segura de HTTP. Utiliza una capa adicional de seguridad llamada SSL (Secure Sockets Layer) o TLS (Transport Layer Security) para cifrar los datos que se transmiten entre el cliente y el servidor. Esta capa de cifrado asegura que los datos no puedan ser leídos por personas no autorizadas, lo que brinda una mayor privacidad y seguridad.

La seguridad proporcionada por HTTPS es especialmente importante cuando se trata de transmitir información confidencial, como contraseñas, datos de inicio de sesión, información financiera o cualquier otro dato sensible. Los sitios web que utilizan HTTPS muestran un candado en la barra de direcciones del navegador y la URL comienza con "https://" en lugar de "http://".

## 13.2-Versiones de http:
- HTTP/0.9: Esta fue la primera versión del protocolo HTTP, introducida en 1991. Era una versión muy simple y solo permitía solicitar y recibir documentos HTML sin ningún encabezado adicional (no sortaba headers) y solo permitía el método GET.
- HTTP/1.0: Fue lanzada en 1996 y agregó características más avanzadas, como la capacidad de enviar diferentes tipos de contenido, encabezados de solicitud y respuesta, y códigos de estado para indicar el resultado de la solicitud. Sin embargo, esta versión tenía limitaciones de rendimiento y no era muy eficiente en la transferencia de recursos web. Actualmente se sigue utilizando pero sobre todo en servidores PROXY. Este tipo de protocolo soporta GET,HEAD y POST. 
- HTTP/1.1: Esta versión, publicada en 1999, es ampliamente utilizada actualmente. Introdujo mejoras significativas en la eficiencia y el rendimiento en comparación con HTTP/1.0. Presentó la capacidad de mantener conexiones persistentes, lo que permitía la reutilización de la misma conexión para varias solicitudes y respuestas, lo que reducía la sobrecarga de establecimiento de conexión. Es la más utilizada a día de hoy. Conexiones persistentes activada por defecto. Pipeline. 
- HTTP/2.0: Lanzado en 2015, HTTP/2 es una versión más avanzada y optimizada del protocolo. Proporciona mejoras en la velocidad de carga de las páginas web al introducir la multiplexación, que permite enviar múltiples solicitudes y respuestas en paralelo sobre una única conexión. También introduce la compresión de encabezados y otros mecanismos para reducir el consumo de ancho de banda y mejorar el rendimiento en general.
- HTTP/3.0: Es el más moderno de todos que sustituye el protocolo TCP por UDP.

## 13.3-Métodos de petición HTTP:
(*Importantes)
- GET*: Obtener datos a través de una request y una response. Este método se utiliza para solicitar recursos, como páginas web, imágenes o archivos, desde un servidor. La solicitud GET envía los parámetros a través de la URL y el servidor responde con el recurso solicitado.

- POST*: Este método se utiliza para enviar datos al servidor para su procesamiento y crear nuevos regursos. Por lo general, se utiliza cuando se envían formularios web o se realiza alguna acción que implica enviar información al servidor. Los datos se envían en el cuerpo de la solicitud en lugar de la URL.

- PUT*: Editar. Este método se utiliza para enviar datos al servidor y actualizar un recurso existente en el servidor. Permite enviar un recurso completo o solo partes del mismo.

- DELETE*: Eliminar. Como su nombre indica, este método se utiliza para solicitar al servidor que elimine un recurso específico.

- PATCH*: No editando todo el recurso pero de forma parcial. Similar al método PUT, PATCH se utiliza para enviar datos al servidor y realizar modificaciones parciales en un recurso existente.

-TRACE: Solicita al servidor que introduzca en la respuesta todos los datos que reciba en la petición. Se suele utilizar para desarrollo. 

- HEAD: Igual que el GET pero no recibimos los datos, solo recibimos los encabezados. Más rápido que GET.

- OPTIONS: Nos devuelve todos los métodos HTTP que el servidor soporta

- CONNECT: Se utiliza para saber si una web está disponible. 

- UPDATE: Modifica el contenido y las versiones obsoletas de un recurso versionado. -> Actualiza

- MOVE: Mover un recurso de una URI a OTRA. Sería comohacer un DELETE + POST

- MKCOL: Crea una colección en la URI especificada. 

- PROPFIND:  Obtiene las propiedades de un recurso especificado. 

- PROPATCH: Modifica las propiedades de un recurso

- MERGE: Une dos recursos en una petición. 

- LABEL: Modificar la etiqueta de un recurso. 

## 13.4-Respuestas HTTP:

Página para ver visualmente los errores o respuestas Http -> [https://httpcats.com/]