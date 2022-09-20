# consultas2.sql

![tabla_tabla](/images/total.png)

## CONSULTAS SQL

1.Traer el nombre, Cédula y Salario de un empleado, ordenando los campos
de la siguiente manera: Ascendente por nombre y descendente por cedula.

`SELECT NOMBRE, CEDULA, SUELDO FROM EMPLEADOS wHERE (CIUDAD='MEDELLIN')ORDER BY NOMBRE;`

![consulta1](/images/consulta1.png)

`SELECT NOMBRE, CEDULA, SUELDO FROM EMPLEADOS WHERE (CIUDAD= 'MEDELLIN')ORDER BY CEDULA DESC;`

![consulta1.1](/images/consulta2.png)

2. Traer el nombre y salario de los primeros 25 empleados cuyo sueldo es
mayor de $600000 ordenándolos en forma ascendente por el numero de
cedula.

`SELECT TOP 2 nombre, sueldo FROM Empleado WHERE(sueldo>600000)ORDER BY cedula;`

![consulta2](/images/consulta3.png)

3.Mostrar el nombre, id y cedula de los primeros 15 empleados cuyos nombres sean distintos. Orden la consulta en forma descendente por cedula.

`SELECT DISTINCT TOP 15 nombre, id, cedula FROM Empleado ORDER BY cedula DESC;`

![consulta3](/images/consulta4.png)

4.Entregar los primeros 15 empleados con nombre y cedula cuya ciudad sea BOGOTA. Se necesita que los encabezados de las columnas tengan los siguientes titulos:

a. Para el campo NOMBRE ----- RAZON SOCIAL
b. Para el campo CEDULA-----IDENTIFICACION
C. Ordene la lista en forma descendente por cedula

`SELECT TOP 15 NOMBRE AS "RAZON SOCIAL", CEDULA AS "IDENTIFICACION" FROM EMPLEADOS WHERE (CIUDAD = BOGOTA)ORDER BY CEDULA DESc;`

![consulta4](/images/consulta5.png)

5.Realizar una consulta que entregue el nombre, identificación, sueldo, edad de los empleados cuyos sueldos estén entre $800000 y $1200000 y cuyas edades estén entre los 23 y 30 años.


`SELECT NOMBRE, CEDULA, SUELDO, EDAD FROM EMPLEADOS WHERE (SUELDO BETWEEN 800000 AND 1200000 AND EDAD BETWEEN 23 AND 30)`

![consulta5](/images/consulta6.png)

6 Realizar una consulta que muestre nombre, cedula y salario de los empleados Cuyo nombre comience por la letra c. ordene esta lista por salario en forma descendente.

SELECT NOMBRE, CEDULA, SUELDO FROM EMPLEADOS WHERE (NOMBRE LIKE
C)ORDER BY SUELDO DESC

![consulta6](/images/consulta7.png)