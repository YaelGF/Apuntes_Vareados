# Between 
Una consulta que se encuentre entre los parametros 1 and 2
````SQL
select * from table where campo between campo1 and campo2;
````
 ## Se pueden usar los operadores logicos
> mayor que
< menor que
>= mayor o igual a
<= menor o igual a 
!= diferente a

## Consultas para el usuario
En esta consulta te devuelve todo registro que contenga gmail dentro de el:
````SQL
select * from tabla  like '%gmail%';
````

En esta consulta te devuelve todo registro que termine en gmail:
````SQL
select * from tabla like '%gmail';
````

En esta consulta te devuelve todo registro que inicie con gmail:
````SQL
select * from tabla like 'gmail%';
````


## Consultas acomodadas de manera ascendente y descendente
De manera ascedente:
````SQL
select * from tabla order by campo asc;
````

De manera descendente:
````SQL
select * from tabla order by campo desc;
````

## Consultas en base al maximo numero o el minimo
Maximo:
````SQL
select max(campo) as titulo from Tabla;
````

Minimo:
````SQL
select min(campo) as titulo from Tabla;
````

nota: el titulo que esta despues del as se refiere al sobre nombre que va a tener el campo

## Poner sobre nombres a las tablas
````SQL
select columna as apodo from tabla;
````
