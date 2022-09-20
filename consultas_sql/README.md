1. Traer el nombre, Cedula y Salario de un empleado, ordenando, los campos de las siguiente manera: Ascendente por nombre y descendentes por cedula.

`SELECT NOMBRE, CEDULA, SUELDO FROM EMPLEADOS WHERE (CUIDAD='MEDELLIN') ORDER BY NOMBRE`

![consulta 1](img/consulta1.png "consulta 1")
![consulta 1_2](img/consulta1_2.png "consulta 1_2")

2. Traer el nombre y el salario de los primeros 25 empleados cuyo sueldo es mayor de $6000000 ordenandolos en forma ascendente por el numero de cedula.

`SELECT TOP 25 NOMBRE, SUELDO FROM EMPLEADOS WHERE (SUELDO>6000000)ORDERNBY CEDULA`

![consulta 2](img/consulta2.png "consulta 2")

3. Mostrar el nombre,id y cedula de los primeros 15 empleados cuyos nombres sea distintos. Orden la consulta en forma descenente por cedula. 

SELECT DISTINCT TOP 15 NOMBRE,ID,CEDULA FROM EMPLEADOS ORDEN BY CEDULA DESC;

![consulta 3](img/consulta3.png "consulta 3")

4. Entregar los primeros 15 empleados con nombre y cedula cuya ciudad sea BOGOTA. Se necesita que los encabezados de las columnas tengan los siguientes titulos: 

a. Para el campo NOMBRE -------RAZON SOCIAL 
b. Para el campo CEDULA -------IDENTIFICACION 
c. Ordene la lista en forma descendente por cedula 

`SELECT TOP 15 NOMBRES AS "RAZON SOCIAL", CEDULA AS "IDENTIFICACION" FROM EMPLEADOS WHERE (CIUDAD='BOGOTA')ORDER BY CEDULA DESC`

![consulta 4](img/consulta4.png "consulta 4")

5. Realizar una consulata que entregue el nombre, identifacacion, sueldo, edad de los empleados cuyos sueldos esten entre $800000 y $1200000 y cuyas edades esten entre los 23 y 30 años.

`SELECT NOMBRE, CEDULA, SUELDO, EDAD FROM EMPLEADOS WHERE (SUELDO BETWEEN 800000 AND 1200000 AND EDAD BETWEEN 23 AND 30`

![consulta 5](img/consulta5.png "consulta 5")

6. Realizar una conslta que muestre nombre, cedula y salario de los empleados cuyo nombre comience por la letra c.ordene esta lista por salarioen forma descendente.

`SELECT NOMBRE,CEDULA,SUELDO FROM EMPLEADOS WHERE (NOMBRE LIKE'C%')ORDER BY SUELDO DESC`

![consulta 6](img/consulta6.png "consulta 6")