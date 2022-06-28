## Foreign key
````SQL
create table name(
id int not null auto_increment,
llave_foranea int not null,
primary key(id)ñ
foreign key(llave_foranea) references tabla2(campo)
);
````

## Renombrar una tabla

````SQL
rename table before to after;
````



