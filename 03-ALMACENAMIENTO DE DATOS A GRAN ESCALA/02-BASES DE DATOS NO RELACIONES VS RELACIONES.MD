# BASES DE DATOS RELACIONALES VS NO RELACIONALES


### Bases de datos relacionales

  las bases de datos relaciones estructuran los datos en tablas, de esta forma se evita la duplicidad de datos y son bases de datos que permiten la consistencia de los datos, usan transaciones que son el 
   
    - acid

     - Atomicity
       - Las operaciones se ejecutan de forma completa o no se ejecutan en absoluto

     - Consistency.
       - Las operaciones se ejecutan de acuerdo con las reglas de la base de datos

     - Isolation.
      - Las operaciones no se afectan entre sí, incluso si se ejecutan simultáneamente

     - Durability.
      - Las operaciones persisten y no se pueden deshacer, incluso si el sistema falla. 

las bases de datos relacionales usal el lenguaje SQL que es muy potente, las ***Desventajas*** son que son mas lentas pero porque tienen mucha consistencia son ideales de usar para cuando necesitamos mucha consistencia y seguridad en ejecucion de consultas y resulotados,






### Bases de datos no relacionales
 
  las bases de datos no relacionalesexisten de varios tipos clave valor grafos etc dependiendo la necesidad existe una base de datos para esa solucion, estas bases de datos al no ser estructurales se pueden agregar datos en las colleciopnes sin tener que modificar la estructura de la tabla, 
  aunque no tienen transaciona asid por ejemplo se piueden usar con orm

  - Base
    - Basically Available
      - La disponibilidad de prioriza mucho
      - Lecturas y escrituras posibles incluso en fallos parciales o particiones de red.
      - Se busca una consistencia eventual.

   - Soft State
    - Se permite tener información en estados intermedios o transitorios

   - Eventually consistent
    - No se garantiza una consistencia total en todo momento.
    - Lecturas realizadas por diferentes usuarios pueden tener distintos resultados
    - Con el tiempo, se asegura que los datos estén en un estado consistente.
