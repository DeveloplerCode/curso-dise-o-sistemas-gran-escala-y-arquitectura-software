# CQRS Y EVENT SOURCE

 
  cqrs se basa en la separacion de la insercion y las consultas en nuestro sistema
  es decir, se puede usar una base de datos y un modelo 
  para las escrituras y uno para las lecturas, asi podemos evitar 
  joins en sistemas grandes.
   
    
    - comandos
     
      - acciones que realizan una accion en el estado del sistema, 
        y que no devuelve informacion, 
        **ejemplo** escribir un post
    
    - consultas 
     
      - acciones que no alteran el estado del sistema, tan solo
        devuelven datos, 
        **ejemplo** obtener los ultimos diez datos de un post

    
  se pude tener por ejemplo una base de datos de escritura en mysql 
  y otra de lectura en mongodb, la desventaja para este caso 
  es que hay que sincronizar los datos y esto tiene un coste de tiempo
  existen varias formas de sincronizar los datos algunas son.

    
   - Consistencia inmediata.
      - Método síncrono.
   
   - Consistencia eventual.
      - Sincronización asíncrona.

   - Consistencia programada.
      - Sincronización a ciertas horas del día.

   - Consistencia bajo demanda.
      - Se realiza la sincronización cuando se determine necesaria.


 ### event sourcing
  
    sistema que almacena el estado como una secuencia de eventos
    almacena el estado de los eventos en lugar de alamacenar el 
    estado de cada evento, al almacenar toda la secuencia de eventos 
    se puede reconstruir en estado en cualquier momento.