# Principio de Abierto/Cerrado  (OCP)
Este principio refiere que los modulos deben ser abiertos para su extension, donde el comportamiento del módulo puede extenderse y ampliarlo con nuevos comportamientos, pero cerrados para su modificación, ya que si se dispone de una interface estable y bien definida, no deberiamos de modificarla.  
En nuestro sistema, la clase Obra Social, es responsable de determinar si la consulta con el especialista esta cubierta por determinada prepaga.  

## Motivación  
En nuestro Sistema de Gestion de Turnos la clase Obra Social define si dicha prepaga cubre la consulta medica. En este caso, por el momento solo cubre ciertas prepagas, por ejemplo solo Osde, pero si mas adelante se desean agregar mas prepagas para la cobertura, tales como Galeno Y SanCor Salud, sino creamos una extension, deberiamos modificar la clase principal y de esta manera rompemos con el principio mencionado. Por lo tanto, una solucion es agregar la extension IPrepagas, por lo que cada vez que se desee agregar o quitar prepagas solo trabajamos con la extension.    
Un ejemplo de la vida real, puede ser que un medico de nuestro Centro de Salud inicialmente atendia consultas solo de la prepaga OSDE, pero luego llego a un convenio con la prepaga Galeno, por lo que a partir de ahora trabaja con ambas prepagas.    

## Estructura de clases  

![OCP](https://github.com/user-attachments/assets/1bac97f5-e18e-4bde-8633-956ada1c5689)  

[OCP](https://drive.google.com/file/d/1SdUhDH4IlcePEO94dtXZfqtB1DyLaTi_/view?usp=sharing)




