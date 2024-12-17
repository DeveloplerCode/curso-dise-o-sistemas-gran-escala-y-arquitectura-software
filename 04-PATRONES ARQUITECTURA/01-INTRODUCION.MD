# INTRODUCION
 
  ### patrones de arquitectura de software
   
   - Arquitectura multi-layer y multi-tier.
    
     - Organiza un sistema en capas lógicas, donde cada una tiene una función específica.

     - Cada capa se comunica sólo con las adyacentes

     - La multi-tier extrapola los mismos objetivos al plano físico. Despliegue independiente.

 
  - Arquitectura de microservicios.
   
    - Conjunto de pequeños servicios, los cuales se ejecutan de forma independiente.

    - Facilita la división del trabajo entre distintos equipos.

  - CQRS y Event Sourcing.
   
    - CQRS: Separa las lecturas de las escrituras. Modelo optimizado para cada operación.

    - Event Sourcing: almacena todos los cambios del sistema como una secuencia de eventos.