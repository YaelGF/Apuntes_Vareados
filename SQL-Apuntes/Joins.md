## Left join
A diferencia de un **INNER JOIN,**  donde se busca una intersección respetada por ambas tablas, con **LEFT JOIN** damos prioridad a la tabla de la izquierda, y buscamos en la tabla derecha.

Si no existe ninguna coincidencia para alguna de las filas de la tabla de la izquierda, de igual forma **todos los resultados de la primera tabla se muestran**.
![[LEFT_JOIN.png]]
### Ejemplo
````SQL
select t.columna, t2.columna from tabla t left join tabla2 t2 on t.columna = t2.columna;
````
## Right join
En el caso de **RIGHT JOIN** la situación es muy similar, pero aquí se da prioridad a la tabla de la derecha.
![[RIGHT_JOIN.png]]
### Ejemplo
````SQL
select t.columna, t2.columna from tabla t right join tabla2 t2 on t.columna = t2.columna;
````
## Inner join
Lo más usual, lo primero que se suele aprender, es el uso de **INNER JOIN**, o generalmente abreviado como **JOIN**.

Esta cláusula busca coincidencias entre 2 tablas, en función a una columna que tienen en común. De tal modo que **sólo la intersección se mostrará en los resultados**.
![[INNER_JOIN.png]]
¿Por qué ocurre esto? Porque **JOIN** muestra como resultado la intersección de ambas tablas.
### Ejemplo
````SQL
select t.columna, t2.columna from tabla t inner join tabla2 t2 on t.columna = t2.columna;
````
## Cross join
Mientras que **LEFT JOIN** muestra todas las filas de la tabla izquierda, y **RIGHT JOIN** muestra todas las correspondientes a la tabla derecha, **FULL OUTER JOIN** (o simplemente **FULL JOIN**) se encarga de mostrar todas las filas de ambas tablas, sin importar que no existan coincidencias (usará **NULL** como un valor por defecto para dichos casos).
![[CROSS_JOIN.png]]
### Ejemplo
````SQL
select t.columna, t2.columna from tabla t cross join tabla2 t2;
````
## Group by
La cláusula GROUP BY es un comando SQL que se usa para **agrupar filas que tienen los mismos valores** .
La cláusula GROUP BY se utiliza en la instrucción SELECT. Opcionalmente se usa junto con funciones agregadas para producir informes resumidos de la base de datos.

Eso es lo que hace, **resumiendo los datos** de la base de datos.

Las consultas que contienen la cláusula GROUP BY se denominan consultas agrupadas y solo devuelven una sola fila para cada elemento agrupado.La cláusula GROUP BY es un comando SQL que se usa para **agrupar filas que tienen los mismos valores** .

La cláusula GROUP BY se utiliza en la instrucción SELECT. Opcionalmente se usa junto con funciones agregadas para producir informes resumidos de la base de datos.

Eso es lo que hace, **resumiendo los datos** de la base de datos.

Las consultas que contienen la cláusula GROUP BY se denominan consultas agrupadas y solo devuelven una sola fila para cada elemento agrupado.
### Ejemplo
````SQL
select count(id), columna from tabla group by columnaComun;
````
## Having
La cláusula **HAVING** permite seleccionar (o rechazar) un grupo de regristros.
### Ejemplo
````SQL
select count(id), columna from tabla group by columnaComun having count(p.id) >= n;
````