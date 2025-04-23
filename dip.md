# Principio de Inversión de Dependencias (DIP)
Este principio refiere que las entidades de software deben depender de abstracciones y no de implementaciones, ya que si dependemos de una implementación estamos rompiendo el principio debido a que debemos modificar los códigos anteriores.   
En nuestro sistema, podemos mencionar el mismo ejemplo que utilizamos para el principio Abierto/Cerrado, en relación a las prepagas que cubren la consulta con el especialista.  

## Motivación
En el Sistema Gestión de Turnos, en la clase Obra Social, no podemos depender de  una sola prepaga, debido a que si luego comenzamos a aceptar mas prepagas que cubran la consulta, crearemos una interfaz para poder adicionar mas prepagas, por lo que nuestro sistema va a depender de dicha interfaz y no de la implementación.  
Un ejemplo de la vida real, podemos mencionar una compra en un supermercado. Si bien, lo habitual es que al finalizar la compra nos imprima el ticket, pero hoy en día se implemento la opción de que dicho ticket sea enviado a nuestro email. Por lo tanto, se creo una interfaz que se relaciones con las opciones de imprimirlo o enviarlo por email.  
## Estructura de clases
![DIP](https://github.com/user-attachments/assets/f419210a-9a71-472b-b924-c666c14c40e6)
[DIP](https://drive.google.com/file/d/1olVW7aVK_jjLpbrfgj5McHGcIx04Bjtk/view?usp=sharing)

