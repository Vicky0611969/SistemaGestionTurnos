## Principio de Abierto/Cerrado  
Este principio refiere que los modulos deben ser abiertos para su extension, donde el comportamiento del módulo puede extenderse y ampliarlo con nuevos comportamientos, pero cerrados para su modificación, ya que si se dispone de una interface estable y bien definida, no deberiamos de modificarla.  
En nuestro sistema, la clase Obra Social, determina si la obra social cubre la consulta con el especialista.

# Motivación  
En nuestro Sistema de Gestion de Turnos, en la clase Obra Social, esta define si dicha prepaga cubre la consulta medica. En este caso, por el momento solo cubre ciertas prepagas, pero si mas adelante se desean agregar mas prepagas para la cobertura, deberiamos agregarla solo a la extensión creada.  
Un ejemplo de la vida real, puede ser cuando recibimos una notificación de confirmación por una compra que hallamos realizado. La misma, puede estar definida para que nos llegue via email, pero ahora deseamos agregar que la confirmación o notificación nos llegue por la apliacación WhatsApp, o por mensaje de texto común.  

# Estructura de clases  





