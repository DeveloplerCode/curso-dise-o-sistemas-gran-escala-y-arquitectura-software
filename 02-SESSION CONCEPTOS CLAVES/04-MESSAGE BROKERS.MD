# MESSAGE BROKERS

### Que es un message brokers?

 Es una aplicacion de software que permite manejar la comunicacion entre componenetes de aplicaicones distribuidas, actua como intermediario que los mensajes enviados po una aplciacion productora sean recibidos por la aplicacion suscrita receptora de manera eficiente confiable y segura, es una aplciacion independiente "entermediaria".

 ### componente que facilita la comunicacion entre dos modulos de nuestro sistemas

   - Productores. Envían mensajes al message broker.

   - Consumidores. Consumen y procesan los mensajes del message broker.
    
   - Colas. Estructura FIFO en la que se almacenan los mensajes. Se entregan de forma
    síncrona.
    
   - Publicación / suscripción. Los consumidores se suscriben a un topic. Los productores envían mensajes a un topic, el cual será consumido por los suscriptores.


  una de las ventajas es que los datos enviados a las colas se pueden almacenar, y si por ejemplo un consumidor se cae el publicador puede segur enviar los mensaje y cuando el consumidor se recupere podra consumir los datos y viceversa.
  tambien aliviana las cargas largas de trabajo para que el cliente no tenga que esperar 5 10 minutos y asi tenga una buena experiencia de usuario.