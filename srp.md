# Principio de Responsabilidad Única (SRP)
Este principio se puede definir como principio de diseño, donde cada clase debe tener una única responsabilidad, y debe tener solo una razón para cambiar, si debemos modificarla por cada cambio que pueda llegar a ocurrir, se esta violando el  principio.  
Por ejemplo, en nuestro sistema la clase recepcionista tiene mas de una responsabilidad y si deseamos modificar o quitar alguna de sus responsabilidades, deberiamos modificar la clase principal.

## Motivación
En nuestro Sistema de Turnos, en la clase Recepcionista mencionamos cuatro responsabilidades, "Registrar paciente", "Registrar medico", "Agendar turno" y "Cancelar turno". Si en un futuro decidimos que los pacientes y medicos se registren por si solos, habria que modificar la clase Recepcionista.  
Un ejemplo del mundo real podemos mencionar que en el Centro de Salud, implemento un sistema donde cada paciente y medico se registra por si solo, escaneando un codigo QR que lo redirige a la pagina web del centro. Por lo tanto, la recepcionista ya no debe registrarlos. 

## Estructura de clases  
![SRP](https://github.com/user-attachments/assets/3d6d94ec-d398-4135-9466-aadf82bac494)
 
[SRP](https://drive.google.com/file/d/1aP4NKlMW9R5s14P8odXsWOXph1ACaUAt/view?usp=sharing)




