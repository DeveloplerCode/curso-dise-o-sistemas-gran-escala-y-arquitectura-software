# MICROSERVICIOS

  ### Que son los microservicios? 
   
    Los microservicios son un estilo arquitectónico para diseñar 
    aplicaciones donde se dividen en un conjunto de servicios pequeños
    e independientes. Cada servicio se enfoca en una funcionalidad 
    específica del sistema y opera de forma autónoma, comunicándose 
    con otros servicios mediante protocolos ligeros como HTTP o 
    mensajería.

    En los microservicios creamos un servicio para cada cada contexto
    esto tambien trae consigo una mayor escalabilidad porque cada 
    serviico esta aparte se puede tener un equipo para cada microservicio 
    que estan en repositorios diferentes y pueden estar en tecnologias 
    diferentes tambien como node, java, php etc cada microservicio 
    es independiente


### Comunicacion entre microservicios
 
   - api rest 
     
     - simple pero servicios acoplados
     - ambos tienen que estar disponibles para que la comunicacion funcione 
     - suele ser sincrono por defecto


   - sistema de mensajes
    
     - Kafka, RabbitMQ, ActiveMQ etc.
     - desacople total entre los servicios 
     - procesamiento syncrono 
     - Si un sistema no está disponible, el mensaje permanecerá en la cola hasta
       que vuelva a estar disponible, momento en el cual será consumido.


### Cuando usar
  
   - sistemas grandes y complejos con subdominios claramente identificables.
   - disponibilidad de personal para asignar al equipo de cada microservicio
   - sistemas de alta disponibilidad en los que necesitemos escalar fácilmente cada pieza