
# INTRODUCION 

### Aquitectura de software
define la estrucura general del sistema, representa las decisiones de diseño del sistema 
y como se comportan los componentes entre ellos, define las bases sobre las que se construye el software.
una buena arquitectura puede ayudr a:
 
 1. escalabilidad: una arquitectura bien diseñada permite que el sistema soporte una alta demanda de usuario y asi pueda cumplir 
con su proposito de una manera eficiente.

 2. reduce la complejidad: una arquitectura clara y organizada reduce la complejidad del sistema y facilita el mantenimiento y la evolucion.

 3. mejora la flexibilidad: una arquitectura flexible, permite que el sistema se adapte a cambios.

 4. una buena arquitectura ayuda a proteger el sistemas y los datos contra atawues y vulnerabilidades.


### Requisitos funcionales
  recoge las funcionalidades del sistema por ejemplo
    - **Identifica los actores** del sistemas
      - tipos de usuario administrador vendedor comprador
    - **Usuario**
      - permite a los usuarios registrarse e iniciar session
    - **recopilar casos de uso**
      - agregar items al carrito
      - realizar pago del carrito 
    - **Diagramas de flujo**
      - interacion entre componentes y actores en cada caso de uso


### Requisitos no funcionales
   describe las caracteristicas y las restriciones que un software
   debe cumplri como minimo para se aceptable, y estas deben ser medibles, por ejemplo alguno de los siguientes situaciones pueden llevarnos a rediseñar un sistemas,
    - No es lo suficientemente rápido.
    - No es suficientemente seguro.
    - No soporta bien tantos usuarios / peticiones al mismo tiempo.
    - No es sencillo añadir o modificar funcionalidades.
    - No es lo suficientemente fiable
 
  si los requisitos no son medible es dificil rediseñar deacuerdo a ellos por ejemplo

   - la web debe estar disponible funcionando casi todo el tiempo
   - la web debe estar responder rapido a los usuarios

 enves de eso seria mejor describirlo asi:
   - La web debe responder en un tiempo inferior a los 300ms el 90% de las peticiones e inferior a 1s el 99% de las peticiones.

## Restriciones

   - Tecnicas
     - Utilizar un lenguaje o framework específico.
     - APIs o servicios externos.

   - Legales
     - Transacciones en el sector bancario.
     - GDPR en la Unión Europea.

   - De negocios
     - Presupuesto.
     - Tiempo
     - Procesos internos

## Conclusion
  
  La arquitectura de software es muy importante porque de una buena arquitectura de software depende que una aplicacion cumpla con las necesidates para las que fue creado, en si la arquitectura es una idea de como va a funcionar el sistema al recibir los requerimientos, pero hay que tener en cuenta desde las necesidades casos de uso, definicion de interacion entre componentes y restriciones que tiene el sistema.
 
