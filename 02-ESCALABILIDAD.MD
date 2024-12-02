
# ESCALABILIDAD

### Que es en escalabilidad?
 
 la escalabilidad es la capacidad de un sistema para soportar mas carga añadiendo recursos sin ver afectado su rendimiento
 > ***es impresendible un buen rendimiento***

 > No es suficiente que rinda bien bajo ciertas condiciones
  debe hacerlo siempre bajo cualquier contexto


### Escalamiento vertical?

escalamiento vertical es aumentarle mas recursos a la maquina,
es decir mas memoria ram, mas disco duro etc.
 
 - ventajas
   - facil de implementar

 - desventajas 
   - no tolerante a fallos 
   - limite de recursos solo se puede aumentar hasta cierto punto


### Escalamiento horizontal?

escalamiento horizontal, es añadir mas servidores y asi podemos
ejecutar multiples instacioas de nuestros servicios, 

- ventajas
   - no tiene limite teorico
   - es tolerante a fallos (si se cae uno usa otro)

- desventajas 
   - puede ser necesario adaptar el codigo 
   - mayor complejidad


### Gestion del estado?

Hay dos formas de gestionar el estado
 - servicios stateful.
 - Servicios stateless.


### Stateful
 
 este tipo de estado es el almacena informacion en el lado 
 del servidor, por ejemplo el login, por parte de informacion que se guarda en el servidor, el servidor sabe si el usuario 
 esta legitimamente logiado, la desventaja es que no escala bien
 horizontalmente ya que si realiza peticiones a otro servidor
 no va a tener informacion del usuario y por eso va a dar 
 errores.

  - No escalan bien horizontalmente.
  - Podríamos redirigir a los usuarios a un único servidor.
  - No existiría tolerancia a fallos.


### Stateless

 este tipo de estado no guarda informacion en el lado del servidor, es el "jwt" por ejemplo es muy bueno escala bien
 horizontalmente 

  - se almacena en el cliente (cookies).
  - Almacenes de datos. Todos los servidores tienen acceso.


### Escalabilidad organizacional

 es vital poder añadir nuevos integrantes al equipo 
 de una manera rapida y sencilla, se puede asignar un solo reporitorio para todo el proyecto si el proyecto es pequeño no hya problema, peri si es un proyecto grande puede pasar que al realizar cambios en el codigo afecte otra parte, se puede dividir el proyecto por servicios en repositorios separados, y que cada grupo d epersonas trabaje en una funcionalidad y asi no se va a haber afectado otras partes del codigo, este es un ejemplo de que es escalabilidad organizacional.
  
  - buen proceso de onboarding.
  - buena documentación.
  - seguimiento del nuevo integrante.
  - pair programming.
  - Código limpio y legible.


### Resumen

 podemos utilizar los tres tipos de de estrategias es decir
 una no es excluyente una de la otra, se pueden combinar 
 todos los tipos de estrategias, es importante aclarar que no hay relacion directa entre los recursos y la carga, tener el doble de recursos no significa tener el doble de resultados, 

  > podemos llegar a una situacion en la cual añadir mas recursos puede significar que empeore la situacion.



 



  
