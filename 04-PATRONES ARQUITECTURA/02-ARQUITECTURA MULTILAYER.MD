# ARQUITECTURA MULTILAYER
 
  La **arquitectura multilayer** (o de múltiples capas) es un modelo de diseño de software que organiza las responsabilidades de una aplicación en capas separadas, cada una con una función específica. Este enfoque permite una mejor separación de preocupaciones, escalabilidad, mantenimiento y flexibilidad en el desarrollo de sistemas.

  - todo el codigo del sistema esta en un unico componente

  - dividido en capas logicas, habitialmente en 3
   
    - capa de presentacion (frontend)
    - capa de logica de negocios (backend logica)
    - capa de acceso a datos (backend conexion query db)


  arquitectura multi-tier

  También está dividido en niveles. No está limitado, pero lo habitual son los mismos tres niveles. Multi-tier: Enfatiza la distribución física de las capas en diferentes servidores o entornos, como cliente, servidor de aplicaciones y servidor de base de datos.

   - cliente ( presentacion tier )

    - es el nivel con el que interactua el usuario
    - Incluye interfaces gráficas (web, móvil, escritorio) y lógica de presentación.
    - Ejemplo: Navegador web o aplicaciones móviles.

   - Servidor de aplicaciones (Application Tier)

    - Maneja la lógica del negocio y el procesamiento de datos.
    - Puede incluir API REST, middleware o microservicios.
    - Ejemplo: Un servidor que ejecuta Node.js, Spring Boot, Django, o Ruby on Rails.

   - Servidor de base de datos (Data Tier):

    - Responsable del almacenamiento y gestión de datos.
    - Incluye bases de datos relacionales o NoSQL.
    - Ejemplo: PostgreSQL, MongoDB, Redis.


    como tal la diferencia es :

    **multilayer** todo el codigo en una sola aplciacion

    **multi-tier** es parecida a la multilayer por capaz
    pero aqui por ejemplo el front se desplega en un servidor,
    y el backend en otro comoun api rest
