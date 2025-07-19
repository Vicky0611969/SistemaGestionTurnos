# Abstracción
La abstracción consiste en simplificar la complejidad del mundo real modelando solo los aspectos esenciales relevantes para el sistema. Los objetos abstractos representan entidades del dominio de aplicación y sus interacciones, lo que facilita la comprensión y el diseño del software. 
Su importancia en el diseño orientado a objetos es que permite centrarse en las caracteristicas y comportamientos importantes para el sistema, ignorando los detalles innecesarios y mejora la organización y claridad de los modelos, facilitando su mantenimiento y escalabilidad.
Podemos decir que se relaciona con el Principio de Responsabilidad Única, ya que al abstraer cada clse tiene una única responsabilidad esencial. Asimismo, se usa en patrones como Factory Method, ya que crea objetos a partir de clases abstractas.

## Ejemplo en el Proyecto
![Abstraccion](https://github.com/user-attachments/assets/ba7b355a-59c2-4071-bee7-b659bd788f11)
[Abstraccion](https://drive.google.com/file/d/1Gi27pQN3YWjDA5SK2Mj1WQCnCXDiYr_y/view?usp=sharing)    

En el diagrama se observa que la clase Persona representa una abstraccion general de todas la personas del sistema. Contiene atributos y mètodos comunes, y no se implementa por sí sola, sino que las clases medico y Paciente heredan de ella y agregan sus características especificas.  
Estas clases aplican abstracción porque modelan solo los aspectos esenciales de las personas el sistema. La clase Persona define lo general y sus subclases implementan lo particular, reduciendo la duplicación de código y simplificando el diseño, lo que facilita el mmantenimiento y extension del sistema de turnos.  

## Ejemplo de código
public class Persona {    
    private String nombre;     
}    
public class Paciente extendes Persona {    
    private int dni;    
}    
public class Medico extendes Persona {    
    private int matricula;    
}    
Este fragmento demuestra la abstracción, ya que la clase Persona define los atributo generales, como nombre, apellido, telefono, y las clases Paciente y Medico heredan de ella, agregando solo sus atributos especificos, como dni y matricula. Así representan solo las caracteristicas esenciales de cada clase, ignorando detalles innecesarios.
