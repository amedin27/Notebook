# 10- Colas de mensajes
(Message queuing). Imagina que nosotros tenemos un Front-End que se tiene que conectar con un Back-End. Una vez conectado, el Back-End me devuelve una respuesta. Cada vez que queremos obtener info hacemos una llamada al Back y obtenemos una respuesta. Si solo hay una llamada no pasa nada. Pero ¿qué pasaría si en vez de tener una llamada tenemos 500?. 

Puede ser que el Back-End tenga una respuesta normal hasta que los recursos que están distinados al Back-En empiezan a llegar a su límite. En ese momento, si llega otra llamada más, como está colapsado no se llegue a producir y tengamos un fallo. Esto no nos lo podemos permitir. Es mejor que exista un delay que nos falle la app. 

Por eso, se plateó la cola de mansajes. La cola de mensajes no es más que una interfaz intermedia que va almacenando en caché los mensajes que van llegando para después llevarlos de forma ordenada al Back-End para no colapsar el sistema. La cola sería la que se conecta directamente al Back. Es la cola la que gestiona los mensajes. 

Esto lo que nos permite es disociar las apps con una interfaz intermedia a través de un sistema asíncrono para controlar estos mensajes. 

## 10.1- ¿Qué es un mensaje?
Es una información, unos datos que deben ser tranmitidos del Front al Back. Por ejemplo
- Archivos, texto, documentos XML, documentos JSON... 

## 10.2- Tipos de estructuras
- Cola de mensajes punto a punto: En una cola de mensajes punto a punto, los mensajes se envían desde un emisor (producer) a un receptor específico(consumer). Solo el receptor designado recibirá el mensaje. Todo se gestiona a través de la cola (Queue). Aquí se gestiona de 1:1

- Cola de mensajes suscriptor: En la cola de mensajes subscriptor es una relación de 1 a N donde N es el número de suscriptores. En este caso tenemos el Publisher ( quien envia el mensaje), la cola que administra los mensajes y el Subscriber ( muchos) quiénes reciben los mensajes. 

## 10.3- Ventajas de utilizar colas
- Disociación de apps
- Especialización de las apps
- Escalabilidad
- Procesamiento
- Evolución

## 10.3- Proveedores
- Rabbit MQ
- Redis: Sitema Open Source que nos proporciona un servico de cola de mensajes