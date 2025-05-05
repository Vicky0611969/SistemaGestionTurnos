# Principios de Segregación de Interfaces (ISP)
Este principio establece que muchas interfaces cliente especificas son mejores que una interfaz de propósito general. No se debe obligar a los clientes a utilizar interfaces que no necesitan.  
En nuestro sistema, podemos tener una interfaz de Gestion de Turnos que contenga solicitar turno, cancelar turno, confirmar turno, que no son necesarias para todas las clases.

## Motivación
En el Sistema de Gestión de Turnos, podemos tener una Interfaz general de Gestion de Turnos, que contenga distintas acciones como las mencionadas anteriormente, que no todas son utilizadas por las clases, tales como Especialista, Paciente y Recepcionista. Una posible solución es realizar interfaces mas pequeñas que contengan una responsabilidad cada una, para no obligar a los usuarios a utilizarlas. Como por ejemplo, el especialista no es necesario que lo obliguemos a utilizar la funcion de solicitar turno.  
En un ejemplo de la vida real podemos mencionar a los telefonos celulares, pueden tener una interfaz general que contenga navegar en la web, realizar llamadas, y conectarse al WIFI. En este caso, no todos los telefonos celulares tienen acceso a la web, o conectarse a WIFI, los telefonos antiguos no poseen esas caracteristicas. Entonces, como solución creariamos interfaces mas pequeñas de cada acción para luego relacionarlas con el dispositivo que corresponda.   

## Estructura de clases
![ISP](https://github.com/user-attachments/assets/a7257106-82b1-4bea-97c6-f746052ce882)   
[ISP](https://drive.google.com/file/d/1B8hLt0AgeYZ3EBklAOsIxdcsNI2qW6Yf/view?usp=sharing) 




