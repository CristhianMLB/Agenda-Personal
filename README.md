# Agenda-Personal
Agenda personal, prueba de programación para Eciglogistica. El programa es una base de datos programada en lenguaje SQL.
Se encuentra en el proyecto archivos y diagramas del programa MySQL Workbench.

La base de datos consta de 4 tablas.
Tenemos la tabla "Contactos" en la que podemos almacenar todos los datos necesarios de los contactos que agreguemos a la lista.
Como datos tenemos el DNI del contacto añadido que es Clave Primaria y es clave ajena en la tabla "Invitados_Cita", el nombre que es
no nulo, los apellidos, el teléfono que es no nulo, el correo, el grupo al que pertenece que es clave ajena de la tabla "Grupo", y
fecha de nacimiento.
Tenemos también la tabla "Grupo". En ella tenemos el campo Nombre que es la Clave Primaria y es clave ajena en la tabla de "Contactos",
y el campo Descripción donde podemos poner una pequeña anotación para definir cada grupo.
La siguiente tabla es "Calendario". En ella tenemos idCalendario que es Calve Primaria de la tabla, auto-incremental y clave ajena
en la tabla "Invitados:Cita", el campo Fecha que es no nulo, el campo Hora, el campo Notas, y el campo Estado que es un enumerado de
4 posibilidades (Pendiente, Completado, Anulado,Retrasado).
Finalmente esta la tabla "Invitados_Cita". En ella tenemos idCalendario que es clave ajena de "Calendario", y DNI, que es clave ajena
de la tabla Contactos.
