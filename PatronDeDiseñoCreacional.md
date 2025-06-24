# Aplicacion de Patron de Diseño creacional - Factory Method  

Los patrones creacionales proporcionan mecanismos de creación de objetos que incrementan la flexibilidad y la reutilización de código existente, evitando el acoplamiento rígido entre códigos y objetos. En particular, el patrón Factory Method permite que el sistema este abierto a la extensión pero cerrado a la modificacion, lo que se relaciona directamente con el principio SOLID de abierto/cerrado. Gracias a esta estrategia, se evita modiciar el codigo existente al agregar nuevas prepagas.       
El problema a resolver es evitar modificar el sistema cada vez que se quiere agregar una prepaga. El propóstio del patrón Factory Method, es delegar la creación de objetos a clases fábrica, evitando instanciaciones directas. Esto permite mantener el código abierto a nuevas extensiones sin alterar clases ya existentes.    
## Motivación  
En nuestro sistema de gestion de turnos, la clase Obra Social nos informa si una consulta esta cubierta o no por una prepaga. En un primer momento, nuestro consultorio solo cubria la prepaga Osde, pero al momento de agregar otras obras sociales, por ejemplo Galeno y SancorSalud, observamos el problema en nuestro sistema. Es por ello, que al intentar modificar la clase Obra Social para ir agregando mas prepagas, se rompe el principio abierto cerrado de los principios Solid.   
Por lo tanto, se definió una interfaz IPrepaga que es implementada por todas las prepagas que se deseen agregar, utilizando luego el patrón Factory Method, creando una jerarquía de clases de fábrica para instanciar prepagas sin acoplarse a clases específicas.  
Las clases implementadas son el Producto interfaz, que en nuestro caso seria IPrepaga, que es comun para todas las prepagas que utilizaremos; la clase productos concretos serian las prepagas implementadas; la clase creador abstracto, es quella que define la implementacion de las prepagas, que retorna nuestra interfaz; y las clases creadores concretos que implementan el creador abstracto para devolver una instancia de su prepaga correspondiente.

## Estructura de Clases
![Patron Factory](https://github.com/user-attachments/assets/c53fd822-cf9c-475c-ac8f-7af57d9d6380)

[Patron Factory](https://drive.google.com/file/d/12C6U1ze_WPSeH8dh97WdoLF5G0WzcMIC/view?usp=sharing)




