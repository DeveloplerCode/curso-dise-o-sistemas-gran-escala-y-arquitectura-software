# FIABILIDAD

### Que es fiabilidad?

Es la probabilidad de que un software se ejecute durante determinado tiempo, sin que se produzca una interrupcion u fallos.

  - uptime
    - tiempo que nuestro sistema esta operativo
  
  - downtime
    - tiempo que nuestro sistema no esta operativo

  - disponibilidad
    - disponibilidad (%) = uptime / tiempo total


### Que sucede si tenemmos multiples servicios ?
  
  - uptime = (n° servicios operativos / n° servicios totales) * tiempo.
  - No tiene en cuenta el porcentaje de uso de cada uno.

 - uptime = (n° servicios operativos / n° servicios totales) * tiempo.
   No tiene en cuenta el porcentaje de uso de cada uno.

 - uptime = (n° peticiones exitosas (est.) / n° peticiones totales   (est.)) * tiempo. No tiene en cuenta la relevancia de cada servicio.



    
### Otras metricas

 - Mean Time Between Failures (MTBF)
   - Tiempo medio entre fallos de nuestro sistema. Nos interesa un MTBF alto.

 - Mean Time To Recover (MTTR)
   - Tiempo medio para recuperar el sistema de algún fallo. Nos interesa un MTTR lo más bajo posible.


### Alta disponibilidad
 
  que significa un sistema con alta disponibilidad?
  
  - 90% ?
  - 92% ?
  - 97% ?
  - 100% ?

  los clientes requieren que el sistema sea 100% disponible pero esto es algo que no es posible debido a que se pueden presentar varios tipos de fallo por ejemplo

   - fallos humanos
   - fallos de hardware
   - fallos de terceros
   - mantenimientos

 los fallos son inevitables pero para mitigar esto lo que debemos es tener un plan de de mitigacion como por ejemplo
  
   - prevencion
   - deteccion 
   - recuperacion

### Prevencion de fallos
 
  - punto único de fallo (Single Point Of Failure)
    
    para este caso es el elemento que si falla el sistema quede inoperativo

    - servidor
    - BBDD 
    - servicio de terceros

    es importante eliminar el punto unico de fallos pero como se hace
    para este caso una posible solucion seria

     - aplicar redundancia
     - multiples servidores (escalado horizontal)
     - multiples BBDD


### Deteccion de fallos
  
   una deteccion de fallos es vital porque 

    - aviso a interesados
    - puesta en marcha de estrategias de contencion y recuperacion

  nuestro sistema debe ser capaz de detectar de detectar falos parciales y realizar acciones de contencion como por ejemplo

   - redirigir el trafico a otros servidores

 por eso es importante la 
  
   - monitorizacion
    
     - automatica
     - equipo dedicado



### Recuperacion de fallos

 la importancia de esto es poder recuoerar la operatividad del sistema de una manera rapida y que el usuario sufra el menor impacto posible

  - apagar por completo el sistema
  - roolback a una version anterior
  - copia de seguridad de los datos

la recupoeracion debe ser lo mas sencilla posible, 

  - una vez recuperado el sistema los fallos deben ser documentados

esto se hace con el fin de crear estrategias para mitigar otra posible falla o tener documentacion para una proxims falla el tiempo de recuperacion del sistema sea corto.

