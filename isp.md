## Principios de Segregación de Interfaces
Este principio establece que muchas interfaces cliente especificas son mejores que una interfaz de propósito general. No se debe obligar a los clientes a utilizar interfaces que no necesitan.  
En nuestro sistema, podemmos tener una interfaz de Gestion de Turnos que contenga solicitar turno, cancelar turno, confirmar turno, que no son necesarias para todas las clases.

# Motivación
En el Sistema de Gestión de Turnos, podemos teneer una Interfaz general de Gestion de Turnos, que contenga distintas acciones como las mencionadas anteriormente, que no todas son ultilizadas por las clases, tales como Especialista, Paciente y Recepcionista. Una posible solución es realizar interfaces mas pequeñas que contengan una responsabilidad cada una, para no obligar a los uduarios a utilizarlas. Como por ejemplo, el especialista no es necesario que lo obliquemos a utilizar la funcion de solicitar turno.  
Un ejemplo de la vida real puede ser

# Estructura de clases



