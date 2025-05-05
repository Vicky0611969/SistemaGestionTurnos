# Principio de Sustitución de Liskov (LSP)  
Este principio nos dice que los objetos de un programa deberían ser reemplazados por instancias de sus subtipos sin alterar el correcto funcionamiento del programa, es decir que si extendemos una clase, se debería poder usar cualquiera de sus clases hijas sin problemas.  
En nuestro Sistema Gestion de Turnos tenemos la clase Paciente, Especialista y Recepcionista, las cuales comparten algunos atributos.

## Motivación
Para evitar caer en un problema que viole el principio de Sustitución de Liskov, tenemos las tres clases mencionadas anteriormente las cuales tienen algunos de sus atributos iguales, tales como el nombre, apellido y correo electronico, entonces podemos crear una clase base denominada Persona, y que de ella surgan las herencias de Paciente, Especialista y Recepcionista.  
Un ejemplo de la vida real, puede ser que nuestro centro de salud, desea enviar una notificacion indicando que el feriado el establecimiento se encontrara cerrado. Se deberia poder enviar la notificacion a todas las personas, sin importar que sean pacientes, medicos o recepcionistas ya que todos ellos heredan de la clase Persona.

## Estructura de clases

![LSP](https://github.com/user-attachments/assets/c9cb47e4-c382-4138-9f9f-f3f38cc193ab)
  
[LSP](https://drive.google.com/file/d/1dUAqkJdo--am0wW_ugP5os1rZu7ja25R/view?usp=sharing)



