## Principio de Responsabilidad Única (SRP)
Este principio se puede definir como principio de diseño, donde cada clase debe tener una única responsabilidad, y debe tener solo una razón para cambiar, si debemos modificarla por cada problema que ocurra, se esta violando el  principio.  
Por ejemplo, en nuestro sistema la clase recepcionista tiene mas de una responsabilidad y si deseamos modificar o quitar alguna de sus responsabilidades, deberiamos modificar la clase principal.

# Motivación
En nuestro Sistema de Turnos, en la clase Recepcionista mencionamos cuatro responsabilidades, "Registrar paciente", "Registrar medico", "Agendar turno" y "Cancelar turno", si en un futuro deseamos quitarle la responsabilidad de Registrar medico, y Registrar paciente, deberiamos realizar dicha modificación en la clase principal, lo que generaria trastornos.  
Un ejemplo del mundo real podemos mencionar a un encargado de edificio. El mismo puede estar encargado de la limpieza de la edificación, de los arreglos internos y de cobrar las expensas a los vecinos del edificio. Aquí, existe mas de una razón para cambiar, ya que se puede contratar una persona para las finanzas y que ésta sea la encargada de cobrar las expensas, o se contrata a una persona que realice los arreglos internos, ya debemos modificar por varias razones la clase principal de EncargadoDeEdificio.  

# Estructura de clases  
![SRP](https://github.com/user-attachments/assets/02e704c8-4b91-458a-925a-5796f4e801cf)
[SRP](https://drive.google.com/file/d/17uYyJn_6kcsq2r6DFEjtZc7SG9PZx7cU/view?usp=sharing)




