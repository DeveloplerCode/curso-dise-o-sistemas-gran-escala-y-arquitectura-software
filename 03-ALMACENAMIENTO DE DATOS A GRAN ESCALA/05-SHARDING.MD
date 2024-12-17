# SHARDING ( PARTICIONADO DE BASES DE DATOS )
 
  ### Que es sharding?

    el sharding o particionado de bases de datos,
    El sharding es una técnica de particionamiento utilizada en bases de datos y sistemas distribuidos para dividir grandes volúmenes de datos en fragmentos más pequeños y manejables llamados shards (fragmentos). Cada "shard" almacena una parte del conjunto total de datos y se distribuye entre diferentes servidores o nodos, lo que permite mejorar el rendimiento, la escalabilidad y la disponibilidad de los datos.

    - Sharding basado en rango.
      
      - Se almacena en cada shard los datos generados en un rango temporal.
      - Muy eficiente para consultas de rango.
      - Desequilibrio en las cargas de cada shard.


    - Sharding basado en hashing.

      - Se aplica función hash a la clave y se asigna a un shard en función del resultado.
      
      - Distribuye uniformemente la carga.
      
      - Ineficiente para consultas por rango. Los datos se encuentran en shards distintos.


    - Sharding basado en listas predefinidas.
    
      - Se establece una lista de valores predefinidos para cada shard. Asignación manual.

      - Nos ofrece un control granular sobre la información que se distribuye a cada shard.

      - Desequilibrio en las cargas de cada shard si las listas no están bien diseñadas.


   el sharding se puede combinar con la replicacion de datos.