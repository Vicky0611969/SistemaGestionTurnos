# Aplicacion de Patron de Diseño de comportamiento - Observer
Los patrones de Diseño de comportamiento definen como interactúan los objetos entre sí, delegando responsabilidades de manera eficiente. El patrón Observer permite que un objeto, sujeto, notifique automáticamente a otros objetos, observadores, cuando cambia su estado sin conocer su tipo exacto.   
Este patrón favorece a los principios SOLID, tales como el principio de Responsabilidad Única en nuestra clase recepcionista, que ya no estaría encargada de las notificaciones, sino que serían los observadores.
Permite que distintas partes del sistema reacciones automaticamente ante ciertos eventos del sistema, sin acomplarse directamente entre sí. En nuestro sistema, es útil cuando se deades que distintas entidades sean informadas cuando un nuevo turno es asignado, cancelado o modificado. 
## Motivación
En el sistema actual, la asignacions, cancelación o modificación de turnos podrían requerir múltiples operaciones conectadas entre sí, generando acoplamiento.   
Al utilizar el patrón Observer, se define una interfaz Observador turno, que será implementada por todas las clases que deban reaccionar ante un cambio en los turnos; se crea una clase GestorTurno, el sujeto, que gestiona la logica principal de los turnos y notifica a todos los observadores suscriptos; y se definen esos múltiples observadores tales como NotificadorPaciente, ActualizadorAgendaEspecialista, RegistrarHistorial, que reaccionan automaticamente cuando se prodece un cambio de estado en un turno. 

## Estructura de Clases
