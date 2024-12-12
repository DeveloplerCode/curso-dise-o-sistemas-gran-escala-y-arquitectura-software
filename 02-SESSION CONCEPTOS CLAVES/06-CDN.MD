# CDN

### Que es un cdn?
 
  Content delivery network, es una red de servidores interconectados 
  que almacenan contenido en cache, en 
  diferentes ubicaciones geograficas, para acelerar 
  el proceso de carga de paginas web.
  permite cachear las peticiones de archivos para que su carga la proxima ves 
  sea mas rapida, y asi brinde una mejor experiencia de usuario, 


### Funcionamiento cdn 

  - el cliente solicita un recurso al cdn 
  - si el cdn no tiene el recurso lo solicita la servidor y lo almacenamos
  - se devuelve el recurso al cliente de forma transparente


### Estrategia pull
 
  el cdn solicita los recursos bajo demanda al servidor 
   
   - si se modifica un recurso en el servidor estaríamos devolviendo un recurso
     desactualizado.
   - debemos establecer un TTL.
  
  si no encontramos la cache o se expiro el tll los oslicitamos al servidor.


### Estrategia push
 
  el servidor envía al CDN los recursos cuando se añaden o modifican

   - el contenido siempre esta actualizado 
   - todas las peticiones estan cacheadas desde la primera
   -necesita mayor mantenimiento de nuestra parte

### Cache en los navegadores
 
  la cache se guarda en los navegadores, de esa manera cuando 
  se realize una peticion que ya se haya echo, la cargara mas rapido.


### Consideraciones cdn 
 
  el servicio tiene un coste importante
   
   - numero de ficheros almacenados 
   - cantidad de datos transmitidos ( tanto hacia los usuario como desde el servidor )