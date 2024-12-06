# INTRODUCION 

### Conceptos claves
 
  implementar funcionalidades como x facebook instagram
  es bastante facil lo dificil es llevar a que una aplicaicon con esste tipo de funcionalidade trabaje bien con millones de usuarios.


### Punto de partida
 
  digamos que por ejemplo tenes una aplicacion donde el cliente realiza las peticiones al servidor el servidor procesa las operaciones y devuelte un resultado, para un sistema sencillo esta bien, este diseño pero primero si como  tiene un unico punto acceso si se cae ya no se podra usar, otra desventaja es que si llegan muchas peticiones el sistema se puede saturar, tamposo se puede escalar "horizontalmente" ya que verticalmente tiene un limite y al llegar a ese limite no s epodra hacer mas.

   - ventajas
     - sencillo y rápido de implementar
     - fácil de mantener
     - aprendizaje

   - desventajas
     - imposible de escalar
     - baja fiabilidad.


### Componentes de un sistema a gran escala

  - load balancer
  - api gateway
  - message broker
  - cahce
  - cdn ( content delivery network )
  - data centers


### Api
 
  - es una interfaz de comunicacion con nuestro sistema
  - expone las operaciones que se pueden realizaar en nuestro sistemas


### Tipos de api
 
  - publica
  - privada
  - partners


### Buenas practicas

 - encapsular las funcionalidad ( no se debe saber como funciona la pai por dentro )
 - desacoplar la api ( separada de front )
 - versionamiento ( ambas versiones deben ser compatibles )
 - paginacion ( no debe devolver una cantidad de datos muy grande )
 - operaciones asincronas ( en segundo plano )