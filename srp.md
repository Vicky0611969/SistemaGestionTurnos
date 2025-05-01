# Principio de Responsabilidad Única (SRP)
Este principio se puede definir como principio de diseño, donde cada clase debe tener una única responsabilidad, y debe tener solo una razón para cambiar, si debemos modificarla por cada problema que ocurra, se esta violando el  principio.  
Por ejemplo, en nuestro sistema la clase recepcionista tiene mas de una responsabilidad y si deseamos modificar o quitar alguna de sus responsabilidades, deberiamos modificar la clase principal.

## Motivación
En nuestro Sistema de Turnos, en la clase Recepcionista mencionamos cuatro responsabilidades, "Registrar paciente", "Registrar medico", "Agendar turno" y "Cancelar turno", si en un futuro deseamos quitarle la responsabilidad de Registrar medico, y Registrar paciente, deberiamos realizar dicha modificación en la clase principal, lo que generaria trastornos.  
Un ejemplo del mundo real podemos mencionar que en el Centro de Salud, se creo un sistema donde cada persona debe registrarse por sì sola. Una vez en el centro la recepcionista solo hace que la persona escanee un codigo QR que lo redirige a la pagina de registraciòn. 

## Estructura de clases  
![SRP](https://github.com/user-attachments/assets/02e704c8-4b91-458a-925a-5796f4e801cf)  
[SRP](https://drive.google.com/file/d/17uYyJn_6kcsq2r6DFEjtZc7SG9PZx7cU/view?usp=sharing)




