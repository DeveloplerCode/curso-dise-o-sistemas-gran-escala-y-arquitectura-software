# TEOREMA CAP
 
 ### Ques es el teorema CAP

  es un sistema distribuido de datos, el cual nos dice que es imposible
  garantizar simultaneamente la consistencia y disponibilidad y la tolerancia 
  a las particiones de red

  - consistencia 
    
    - que todos nuestros nodos de datos ven lo mismo todo el tiempo 
      se devuelve la escritura mas recinete o un error 

  - disponibilidad 

    - prioriza no devolver errores pero no asegura devolver el valor mas 
      reciente 

  - tolerancia a particiones de red 

    - el sistema sigue funcionando apresar que existen problemas 
      de comunicaciones entre diferentes nodos

 ### Tipos de configuraciones

  - configuracion CA ( consistencia y disponibilidad ) 

    - se sacrifica la tolerancia a particiones de red 
    - las particiones de red no dependen de nosostros
    - en la practica no se utiliza 

  - Configuración AP (Disponibilidad y tolerancia a particiones de red)
    
    - se sacrifica la consistencia 
    - si existen particiones de red clientes distintos podran ver informacion diferente 

  - Configuración CP (Consistencia y tolerancia a particiones de red) 
   
    - Se sacrifica la disponibilidad.
    - Si existen particiones de red el sistema no podrá responder a peticiones.