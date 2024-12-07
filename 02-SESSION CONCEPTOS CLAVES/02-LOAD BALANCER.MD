# LOAD BALANCER

### Que es load balancer
 
  un load balancer es un isstema que permite distribuir la carga "peticiones" entre varios servidores

  - **funciones principales**

    - **distribuir trafico:** divide el trafico entre varios servidores para evitar uno solo que reciba toda la carga
    - **alta disponibilidad:** si un servidor falla el balanceador redirige las peticiones a otro que aun funciona
    - **escalabilidad:** facilita el aumento de capacidad agregando mas servidores sin interrumpir el servicio
    - **optimizacion de rendimiento:** puede utilizar algoritmos para enviar las solicitudes al servidor mas cercano o el menos ocupado

 - **algoritmos comunes**

    - **round robin:** envia solicitudes a cada servidor en orden secuencial
    - **least connection:** envia el trafico al servidor con menos conexiones activas
    - **ip hash:** asigna solicitudes en funcion de la direccion ip del cliente
    - **weighted round robin:** da mas carga a ciertos servidores segun su capacidad.

 - **Tipo**
    - **hardware:** dispositivos físicos diseñados específicamente para balancear carga (por ejemplo, F5 Big-IP)

    - **software:** aplicaciones o servicios que actúan como balanceadores de carga (por ejemplo, Nginx, HAProxy, AWS Elastic Load Balancer)

 
 > la ip de nuestros servidores internos sera privada pero el balanceador sera publico ese es el que tendra acceso a nuestro servidores, en realidad esto aumenta algo de latencia pero comparado con los beneficios en mucho mejor.

### Servidor DB 
 
  en este tipo de sistema el servidor de la base de datos ya se pone aparte, es decir los servidores que tienen la logica se conectan con un servidor de SGDB para realizar consultas e inserts 


## Resumen
 
  apesar de que esta es una buena tecnica no es perfecta ya que si el balanceador de carga se cae se pierde el acceso, para mitigar esto se pueden poner otros balanceadores que detecten la falla de uno y entre automaticamente el otro, pero esto trae un problema que configurar esto para que sea automatico no es sencillo, tambien se pueden distribuir sistemas en varias regiones cercanas al usuario y asi mejora el rendimiento.