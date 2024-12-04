
# RENDIMIENTO   

### Que es en resumen?
 el rendimiento es la referencia que se le hace a un software en respuesta a una determidad carga de trabajo, de como se comporta en ciertas condiciones, que tan rapido respode la carga y tiempos de respuesta a las peticiones.


 ### Dos parametros fundamentales para medir el rendimiento
  1. Response time (tiempo de respuesta)
  2. Throughput 


### Response time (tiempo de respuesta) 
 - Tiempo de procesamiento
   - logica de la aplciacion
   - Db conexiones consultas etc

 - Tiempo de espera
   - espera por otras peticiones
   - routers
   - cables
   - switches 
   - ubicacion del servidor

si por ejemplo el servidor esta en europa y la solicitud se hace desde america la peticion pasa por cables routers se demora 1ms
mas el tiempo de alla para aca es otro 1ms en total serian 
2ms y si a eso se le suma 2ms de procesamiento serian 4sm en total
una solucion seria poner fisicamente el servidor en europa asi el timepo de respuesta
disminuye.


### Throughput 
 es el numero de epeticiones que nuestro sistema es capaz de procesar por unidad de tiempo
 y puede ser mas importnte inclusive que el tiempo de respuesta,
 por ejemplo una peticion por usuario demora
 entre 1ms ahora si eso es por cada peticion de usuario y 10 usuarios realizan 
 la misma peticion el tiempo del numero 10 serian mas largo que el del primero


 ### Mediciones en sistemas reales
  en sitemas reales no es sencillo realizar la mediciones 
   - muchos usuario recurrentes 
   - multiples servidores

  para este caso no es recomendar media y mediana porque cada servidor
  tiene una respuesta diferente, para este caso la mejor opcion es usar 
  un instograma y percentiles 


 ### Requisitos
  
  - evitar la media y mediana
  - mejor usar la forma asi: el 99% de las peticiones debe tener una respuesta menor a x ms


  

