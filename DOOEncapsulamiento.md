# Encapsulamiento
El encapsulamiento es el proceso de ocultar la implementación interna de un objeto y exponer solo las interfaces públicas. Esto permite que los objetos mantengan su estado interno protegido de accesos no autorizados, promoviendo así la modularidad y la seguridad del sistema.  
Es importante en el diseño por que protege la integridad de los datos internos del objeto, porque facilita el mantenimiento y la evolución del sistma al limitar el acceso directo a los atributos y detalles internos. Asimismo, permite cambiar la implementación sin afectar a otras partes del sistema que usan el objeto y mejora la claridad y organización del codigo al definir qué es accesible y que no.   
Se relaciona por ejemplo, con el principio de Abierto/Cerrado, ya que al ocultar los detalles internos de una clase, permite extender su comportamiento sin modificar su código existente. En relación a los patrones, podemos mencionar que se relaciona con el patron de Diseño de Comportamiento Observer, ya que este oculta la complejidad interna y expone sólo interfaces públicas para facilitar la interacción y mantener la integridad del sistema. 
## Ejemplo en el proyecto  
![Encapsulamiento](https://github.com/user-attachments/assets/961af442-f47a-4a5a-b2e8-3cf21cbbb0f8)  
[Encapsulamiento](https://drive.google.com/file/d/1uOVHPWhnCEiNocLgGZ_1xQ6gLFBjYwrd/view?usp=sharing)  
Esta clase encapsula informacion sobre la obra social y el plan los cuales no son accesibles desde otras clases. En cambio, la clase expone metodos publicos para interactuar con las otras clases, siendo estas informar si cubre y registrar cobertura medica.  
Esto refleja el encapsulamiento porque oculta los atributos de la cobertura médica, evitando accesos o modificaciones directas, expone solo métodos públicos necesarios para interactuar con ella y protege la integridad de los datos y permite mantener su logica interna sin afectar otras clases.

## Ejemplo en código
private String obraSocial;  
public String getObraSocial(){  
     return obraSocial;  
}
Este fragmento demuestra encapsulamiento porque el atributo obraSocial es privado, no puede ser accedido directamente desde otras clases. Se utiliza un metodo publico getter getObraSocial() para permitir el acceso a su valor.  
Este diseño protege la integridad de los daots internos de la clase, evita accesos no autorizados o modificaciones indebidas y cumple el principio de ocultar la implementacion interna y solo exponer lo necesario.
