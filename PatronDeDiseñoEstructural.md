# Aplicacion de Patron de Diseño estructural - Facade
 Los patrones estructurales explican como ensamblar objetos y clases en estructuras mas grandes, a las vez que se mantiene la flexibilidad y eficiencia de estas estructuras. El patrón Facade proporciona una interfaz que simplifica la interacción con subsistemas complejos, ocultando su implementacioón interna. Se relaciona principalmente con el principio SOLID, Responsabilidad Única, donde cada clase tiene una única responsabilidad específica, por ejemplo registrar pacientes, gestionar turnos, etc.  
El propósito es simplificar el uso del sistema al exponer una interfaz unnificada para varias operaciones internas. De esta manera, podemos resolver el problema de la clase Recepcionista, la que tiene multiples responsabilidades.  
 
## Motivación
En nuestro sistema de Gestión de Turnos, la clase Recepcionista se encarga de múltiples tareas, tales como registrar paciente, asignar turnos, gestionar las coberturas medicas, entre otros, lo que viola el Principio de Responsabilidad Única.  
Para solucionar ese problema, se crea una clase fachada llamada SistemaGestionFacade, siendo esta clase la que centralice las operaciones necesarias para el proceso de atención médica y coordina la interacción entre los susbistemas que se crearán.  
Gracias a ello, la clase Recepcionista puede delegar todas las acciones operativas en la Facade, quedando como un simple cliente de alto nivel del sistema.  
Las clases incorporadas son SistemaGestionFacade, cumpliendo el rol de fachada, que ofrece una interfaz unificada para operaciones del sistema; los subsistemas SistemaRegistro y GestorTurno, y las entidades Paciente, Medico, Turno. 

## Estructura de Clases
