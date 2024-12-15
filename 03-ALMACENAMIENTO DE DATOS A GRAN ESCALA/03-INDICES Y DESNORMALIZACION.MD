# INICES Y DESNORMALIZACION


  ### Indices
   
    los indices en las bases de datos son estructuras que 
    mejoran la velocidad de las busquedas en las tablas, funcionan como unatabla adicional que contiene una copia ordenada de algunos campos, ( o combinaciones de ellos ) junto con punteros a las filas originales.

     - ventajas
      
       - acelera las busquedas y las consultas que utiliza claves especificas

       - mejoran el rendimiento de las operaicones JOIN ORDER BY y GROUP BY

    - desventajas
     
      - ocupa espacio adicional en disco

      - disminuye operaciones INSERT, UPDATE, Y DELETE debido a la necesidad de actualizar los indices



 ### Desnormalizacion
    
    la desnormalizacion es el proceso de combinar varias tablas en una sola para reducir los JOINS (lo inverso a la normalizacion) 

#### razones para desnormalizar
 
    - mejora el rendimiento d electura menos uniones resulta en menos calculos

    - optimizar sistemas con consultas frecuentes y datos raramente actualziados

    - simplicidad en las consultas: las consultas se vuelkven mas faciles de escribir y de leer
   
    
   

    
   