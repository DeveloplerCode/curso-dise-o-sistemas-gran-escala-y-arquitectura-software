  # REPLICACION DE DATOS

   ### Que es replicaicon de datos?
    
     la replicacion de bases de datos es una tecnica, paramantener y copiar datos entre varias ubicaciones, o nodos dentro de un sistema distribuido. un unico servidor de bases der datos en un 
     sistema a gran escala se vera afectdo su rendimiento, se puede 
     volver un cuello de botella.

     - afeta el redimiento
       
       - volumen de peticiones demasiado alto para ser manejado
         por un unico servidor
    
     - afectara la disponibilidad

       - si se cae el servidor BBDD todo nuestro sistema quedara inutilizable


  ### Aspectos positivos de la replicacion de dtos
   
    - mejor rendimiento

      - Escrituras en nodos master y lecturas en slave. Se reparte la carga

    - mayor fiabilidad
     
      - Si un servidor se queda inoperativo nuestros datos permanecerán a salvo en el resto

    - alta disponibilidad
     
      - El sistema sigue disponible aunque uno o varios servidores de almacenamiento se caigan, ya que los datos siguen accesibles en el resto. Se elimina SPF.

    