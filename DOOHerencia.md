# Herencia
La herencia es un mecanismo que permite que un objeto o clase herede propiedades y comportamientos de otro objeto o clase. Esto fomenta la reutilizacion del código y la creacion de jerarquías de clases, donde las clases secundarias (subclases) pueden extender o modificar el comportamiento de las clases primarias (superclases).  
La importancia en el diseño es la reutilización de codigo evitando la duplicacion al cmpartir atributos y metodos y la organizacion y claridad ya que permite modelar relaciones jerarquicas naturales entre entidades.  
Se lo puede relacion con el Principio Sustitución de Liskov, ya que las subclases pueden usarse en cualquier contexto donde se espere una Persona, sin alterar el comportamiento del sistema, por ejemplo un metodo que reciba una Persona puede procesar tanto a un Paciente como un Medico, sin necesidad de cambiar el codigo. En relacion a los patrones, podemos decir que se relaciona con el Patrón Creacional Factory Method ya que el mismo se usa para crear objetos de distintas clases derivadas a partir de una clase base común (Persona). Por ejemplo, cuando el sistema crea un nuevo usuario puede decidir si crear un Paciente o un Medico sin conocer los detalles especificos de cada clase. La herencia garantiza que todas esta clases comparten una interfaz común para ser manejadas uniformemente.  

## Ejemplo en el proyecto
![Herencia](https://github.com/user-attachments/assets/37409dac-cbea-400c-b583-c71070f3baae)  
[Herencia](https://drive.google.com/file/d/1jf0W6JWDjmivLE6dfebKS2_eLmJSSO9M/view?usp=sharing)  
El diagrama muestra que las clases Paciente y Medico son tipos de persona. La clase Persona define los atributos y metodos comunes que son compartidos por las subclases evitando duplicidad de código. Cada subclase extiende el comportamiento de Persona agregado sus atributos y responsabilidades especificas. 

## Ejemplo en código
public class Persona{  
    String nombre;  
}  
public class Paicente extends Persona{  
int dni;  
}  
public class Medico extends Persona{  
int matricula;  
}  
Paciente y Medico heredan de Persona, por lo que ambas clases tienen el atributo nombre sin necesidad de declararlo de nuevo. Cada una agrega su propio atributo, ejemplo dni y matricula, mostrando como la herencia permite reutilizar codifo común y extender con caracteristicas especificas. 
