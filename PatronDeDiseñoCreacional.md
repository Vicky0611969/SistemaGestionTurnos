# Aplicacion de Patron de Diseño creacional - Factory Method  

Los patrones creacionales proporcionan mecanismos de creación de objetos que incrementan la flexibilidad y la reutilización de código existente, evitando el acoplamiento rígido entre códigos y objetos. Se relacionan con los principios SOLID, ya que al usarlos, se promueve un código más limpio, extensible y mantenible, siguiendo las directrices de los princicpios de diseño orientado a objetos.   
El problema a resolver es evitar tener que modificar el sistema cada vez que se quiere agregar una prepaga, siendo ese el propóstio del patrón Factory Method. En lugar de crear objetos directamente, se delega la creación a clases fábrica, permitiendo al sistema mantenerse abierto a extensiones, sin necesidad de alterar clases existentes. 

## Motivación  
En nuestro sistema de gestion de turnos, la clase Obra Social nos informa si una consulta esta cubierta o no por una prepaga. En un primer momento, nuestro consultorio solo cubria la prepaga Osde, pero al momento de agregar otras obras sociales, por ejemplo Galeno y SancorSalud, observamos el problema en nuestro sistema. Es por ello, que al intentar modificar la clase Obra Social para ir agregando mas prepagas, se rompe el principio abierto cerrado de los principios Solid.   
Por lo tanto, se definió una interfaz IPrepaga que es implementada por todas las prepagas que se deseen agregar, utilizando luego el patrón Factory Method, creando una jerarquía de clases de fábrica para instanciar prepagas sin acoplarse a clases específicas.  
Las clases implementadas son el Producto interfaz, que en nuestro caso seria IPrepaga, que es comun para todas las prepagas que utilizaremos; la clase productos concretos serian las prepagas implementadas; la clase creador abstracto, es quella que define la implementacion de las prepagas, que retorna nuestra interfaz; y las clases creadores concretos que implementan el creador abstracto para devolver una instancia de su prepaga correspondiente.

## Estructura de Clases


