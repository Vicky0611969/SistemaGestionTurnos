# Anexo - Introducción al Diseño Orientado a Objetos

## 🟢 Descripción del paradigma orientado a objetos
La programación orientada a objetos es un modelo que se basa en la creación de objetos, los cuales tienen información en forma de campos, para organizar la estructura de un programa. Los objetos son capaces de interacturar y modificar los valores contenidos en sus campos o atributos a través de sus métodos.  
Es importante porque permite:  
-Modularidad: que es la capacidad de divir un programa en modulos independientes, donde cada uno de ellos se enfoca en una tarea especifica, facilitando la reutilización y çcomprensión  
-Reutilización: la reutilización de un codigo permite ahorrar tiempo a largo plazo, evita reinventar la rueda y ayuda a esxribir código mas limpio  
-Mantenimiento: Los cambios de las clases padre se propagan automaticamente en las clases hijas
  
## 🟢 Los cuatro fundamentos de POO  
![WhatsApp Image 2025-03-28 at 23 02 36](https://github.com/user-attachments/assets/e6a6be3c-c68d-46e4-b8ed-df7ba8866702)    

### * Encapsulación:
Proceso de ocultar la implementación interna de un objeto y exponer sólo las interfaces públicas.  
Ejemplo: El usuario solo accede al control remoto y TV, no puede acceder a la estructura interna de los dispositivos.    

### * Abstracción:
Consiste en simplificar la complejidad del munfo real modelando solo los aspectos esenciales relevantes para el sistema  
Ejemplo: El usuario no necesita saber como funciona internamente la TV o el control, solo interactua con ellos para manejar dicha TV.  

### * Herencia:
Mecanismo que permite que un objeto herede propiedades y comportamientos de otro objeto.  
Ejemplo: Existen varios modelos de TV de una misma marca, por lo que una más nueva va adquirir propiedades de los modelos anteriores,facilitando la reutilización del diseño y eficiencia en la producción.  

### * Polimorfismo:
Se refiere a la capacidad de los objetos de una misma jerarquía de clases para responder de manera diferente a un mismo mensaje.  
Ejemplo: Tener el control de la TV, y tener un control Roku asociado a la TV. Al dar la orden de encendido en el control Roku, la TV se encenderá pero con las opciones que da el programa.

## 🟢 Requisitos iniciales del sistema
### 1) Ingresar nuevo paciente:  
El sistema debe permitir ingresar a un nuevo paciente, colocando los datos necesarios del mismo
### 2) Solicitar un turno:  
Debe permitir corroborar la disponibilidad que posee el especialista para otorgar un turno al paciente
### 3) Confirmación de turno:  
Una vez registrado el paciente a un turno con el especialista, se debe notificar dicha acción para confirmar la misma
### 4) Historial de turnos:  
Se debe obtener un historial de los turnos de cada paciente
### 5) Información protegida:   
Se debe contener la información de paciente y medico con acceso solo a personal autorizado  

## 🟢 Casos de uso
### 1) Registrar paciente:    
■ Actor(es): Recepcionista y paciente  
■ Descripción: El paciente desea solicitar un turno por primera vez en nuestro Centro de Salud  
■ Flujo principal de eventos:  
    a) El paciente se comunica telefonicamente con el centro de salud    
    b) La recepcionista ingresa al sistema de turnos y va a la sección de Registrar paciente    
    c) La recepcionista le solicita sus datos personales necesarios para agregarlo al sistema    
    d) Una vez agregados los datos, confirma el ingreso del nuevo paciente  
    e) El sistema genera el nuevo paciente  
    f) El nuevo paciente se guardo exitosamente  
■ Precondiciones: Que sea la primera vez que se registre en el centro  
■ Postcondiciones: Que quede guardado correctamente  

### 2) Solicitar un turno:    
■ Actor(es): Recepcionista y paciente  
■ Descripción: El paciente desea solicitar un turno   
■ Flujo principal de eventos:  
    a) El paciente se comunica telefonicamente con el centro de salud para solicitar un turno      
    b) La recepcionista ingresa a la sección de turnos  
    c) La recepcionista le consulta datos para ingresar a su registro  
    d) La recepcionista le consulta con que especialista desea atenderse        
    d) El paciente le indica especialidad y médico que desea  
    e) La recepcionista verifica disponibilidad del medico y le indica al paciente fecha y horario   
    f) El paciente acepta y toma el turno  
    g) La recepcionista confirma la solicitud  
    h) El sistema guardo exitosamente el turno  
■ Precondiciones: Que el paciente no tenga otro turno el mismo dia y horario    
■ Postcondiciones: Que quede asignado el turno correctamente


### 3) Historial de turnos de paciente:    
■ Actor(es): Paciente  
■ Descripción: El paciente desea consultar sus turnos   
■ Flujo principal de eventos:  
    a) El paciente ingresa a la web o app del centro            
    b) El paciente se dirige a la opción de ingesar como paciente  
    c) Coloca sus datos de ingreso  
    d) Se dirige a la sección Mis Turnos  
    e) Observa los turnos que posee  
    f) Cierra su sesión en el sistema  
■ Precondiciones: Que este ingresado al sistema  
■ Postcondiciones: Que haya verificado sus turnos correctamente  


### 4) Turnos que posee especialista:    
■ Actor(es): Medico  
■ Descripción: El especialista desea consultar los turnos que le fueron solicitados   
■ Flujo principal de eventos:  
    a) El medico ingresa al sistema          
    b) El medico se digire a la opcion de ingreso como especialista  
    c) Coloca sus datos de ingreso    
    d) Ingrese a la sección de su agenda    
    e) Observa los turnos que le fueron solicitados      
    f) Cierra su sesión en el sistema  
■ Precondiciones: Que este ingresado al sistema  
■ Postcondiciones: Que se muestren los turnos que le solicitaron correctamente 

### 5) Cancelar turno:    
■ Actor(es): Paciente y Recepcionista   
■ Descripción: El paciente desea cancelar un turno       
■ Flujo principal de eventos:    
    a) El paciente se comunica con el centro              
    b) La recepcionista atiende el llamado y consulta a que se debe  
    c) El paciente refiere que desea cancelar un turno  
    d) La recepcionista ingresa al sistema y coloca datos del paciente  
    e) La recepcionista colsulta cual turno desea cancelar y confirma la cancelación  
    f) El sistema cancelo el turno  
    g) El sistema informa la cancelación al paciente y especialista  
■ Precondiciones: Que el paciente tenga ese turno asignado  
■ Postcondiciones: Que se haya cancelado correctamente 


## 🟢 Boceto inicial del diseño de clases

![Boceto](https://github.com/user-attachments/assets/a2b8cfbe-6cfb-46f6-992c-b2a7b19aee3c).


[Boceto](https://drive.google.com/file/d/1xY6tKDGEOp5uHEC8Z91a7KsgIuqSwqsc/view?usp=sharing)

