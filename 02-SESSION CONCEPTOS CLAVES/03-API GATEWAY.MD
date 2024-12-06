# API GATEWAY

### Que es un API Gateway?

 Un API Gateway es un componente clave en una arquitectura de software moderna, epecialmente
 basado en istemas distribuidos y microservicios, y actua como punto de acceso unico para 
 los clientes y los accesos internos a los servicios del sistema. de esta manera se puede manejar por ejemplo
 un filtrado de ip en un unico 
   - punto seguridad 
   - autenticidad
   - rate limit 
   - monitorizacion de la api
 
 entre otras

 si se mueve un servicio a otra parte el cliente debe apuntar a ese otro servicio pero si lo hacemos por el api gateway cambiamos la logi en ese solo punto y el cliente no tiene necesidad de hacer cambios.


### Beneficios API Gateway

 - aislamiento de nuestros servicios
 - seguridad y autenticidad centralizada
 - monitorizacion ( de la salud de los servicios )
 - cache y contenido estatico ( puede cachear sin pasar por las peticiones )
 - gestion de trafico y limitacion de acceso

> **se debe evitar llamar los servicios directamente enves de esto se debe llamar por medio del api gateway**

la api gateway no debe tener logica de negocios


### A tener en cuenta

 al funcionar como router por donde pasan las peticiones, esto aumenta la latencia porque al tener que pasar por el api gateway y que la respues tambien tenga que pasar por el api gateway aumenta un poquito la latencia pero por los beneficios que trae usa la api gateway compensa ese corto tiempo de latencia. 

 

