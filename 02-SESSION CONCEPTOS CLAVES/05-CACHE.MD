# CACHE

### Que es la cache?

  es un area de almacenamiento temporalutilizada para almacenar el 
  resultado de operaciones frecuentes y costosas, las peticiones 
  posteriores seran mas rapidas.


### Cache aside
 
  - el cliente realiza una peticion
  - si la cache no tiene el dato se consulta en la db
  - se actualiza la cache con la informacion obtenida
  - se devuelve el resultado al cliente


### Pro y contras 
 
  - **ventajas**

    - reduce el tiempo de lecturas posteriores 
    - minimiza el riesgo de inconsistencia entre la cache y el almacenamiento
      principal
    - muy buena para sistemas read-heavy
    - la cache y la DDBB estan desacopladas


  - **desventajas**

    - cache insonsistente cuando se realizan escrituras
    - latencia adicional durante la recuperacion de datos 
      del almacenamiento principal 
    - la aplicacion es la encargada de realizar el tranajo extra 
      cuando no encontramos la informacion en la cache.


### Read-through  
  
  - El cliente realiza una petición.
  - Si la caché no tiene el dato, consulta
    directamente la BBDD y actualiza la información.
  - Se devuelve el dato a la aplicación de forma transparente.
  - Se devuelve el resultado al cliente.

  - **ventajas**

    - Reduce el tiempo de lecturas posteriores.
    - Minimiza el riesgo de inconsistencia entre la caché y el almacenamiento principal.
    - Muy buena para sistemas read-heavy.
    - Los fallos en caché y posterior consulta a la BBDD ocurren de forma transparente
    - para la aplicación.


  - **desventajas**

    - Caché inconsistente cuando se realicen escrituras.
    - Latencia adicional durante la recuperación de datos del almacenamiento principal.
    - El modelo de la caché y el almacenamiento principal están acoplados.

   
    
### Write-behind / Write-back
  
  - el cliente escribe o actualiza informacion en la aplicacion
  - la aplciacion actualiza la cache con la informacion y la devuelve 
  - se devuelve con exito y se finaliza la conexion con el cliente 
  - la cache acttualiza de forma asincrona el almacenamiento 
    principal con la informacion.


  - **ventajas**

  - Aumentan mucho el rendimiento en sistemas write-heavy.
  - Tolerante a fallos en la BBDD.
  - Puede reducir costes si las escrituras se hacen en batch.



  - **desventajas**

  - No garantiza la consistencia entre caché y BBDD.


### Consideraciones a la hora de usar cache 
  
  - analiza donde y cuando es necesario
    - Tiene un coste asociado e incluso puede resultar perjudicial.
    - ¿Realmente lo necesitas? Observar métricas.
    - ¿Qué tipo de sistema tienes? ¿Read-heavy o write-heavy? ¿La consistencia eventual
      es aceptable?


utilizar una estrategia de cache se debe analizar que tipo de 
estrategia se va a usar y si es necesaria, esto lo que hace 
es que reduce el tiempo de respuesta en consulta a los usuarios
y ayuda a mejorar el rendimiento.
