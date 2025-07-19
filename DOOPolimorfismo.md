# Polimorfismo
El polimorfismo es la capacidad que tienen los objetos de una misma jerarquía de clases para responder de manera diferente a un mismo mensaje o llamada a método. Esto significa que, aunque se invoque un metodo con el mismo nombre, cada objeto puede ejecutar su propia versión adaotada a su tipo especifico.  
La importancia en el diseño orientado a objetos es que permite escribir un codigo generico que puede funcionar con diferentes tipos de objetos sin conocer sus detalles internos, y promueve el uso de interfaces o clases base que definen contratos comunes que luego las subclases implementan según sus necesidades.  
El polimorfismo lo podemos relacionar con el Principio de Segregacion de Interfaces, ya que este principio establece que las clases no deberían estar obligadas a implementar metodos que no utilizan. Por lo tanto, si se respeta ese principio cada subclase implementa solo los metodos que le corresponden, y el codigo puede usar polimorfismo para llamar metodos comunes como por ejemplo getDatos(), y cada uno va a responder segun su implementacion espeifica.  

## Ejemplo en el proyecto
![Polimorfismo](https://github.com/user-attachments/assets/ee8329d8-d277-492a-85e3-c6ef043dabef)  
[Polimorfismo](https://drive.google.com/file/d/1ZupmGQaQj-QPIWdUW86MwdrJzMz5d7P2/view?usp=sharing)  
El diagrama refleja el polismorfismo mediante la jerarquía de herencia entre la superclase Persona y las Subclases Medico y Paciente. Ambas clases comparten atributos y métodos comunes definidos en Persona, cada una puede implementar o redefinir metodos segun sus necesidades especificas. Por ejemplo el metodo solicitarRegistrarse() esta definido en persona, pero podría se implementado de manera distinta en Medico y Paciente para ajustarse a su comportameinto particular. 

## Ejemplo en código
class Persona {  
String solicitarRegistrarse() {  
return "Registro genérico";  
}  
}  
class Medico extends Persona {  
String solicitarRegistrarse() {  
return "Registro médico";  
}  
}  
class Paciente extends Persona {  
String solicitarRegistrarse() {  
return "Registro paciente";  
}  
}  
