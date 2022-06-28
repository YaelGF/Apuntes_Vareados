# Argumentos y parametros indeterminados
Quiza en alguna ocasion no sabemos de antemano cuantos elementos vamos a enviar a una funcion. En estos casos podemos utilizar los parametros indeterminados por posicion y por nombre.

## Por posición
Para recibir un numero indeterminado de parametros por posicion, debemos crear una lista dinamica de argumentos(una tupla en realidad):
````python
def indeterminados_posicion(*args):
	for arg in args:
		print(arg)
indeterminados_posicion(5,"Hola",[1,2,3,4,5])
````
OUT:
````bash
5
Hola
[ 1, 2, 3, 4, 5]
````
## Por nombre
Para recibir un numero indeterminado de parametros por nombre(clave-valor), debemos crear un diccionario dinamico de argumentos:
````python
def indeterminados_nombre(**kwargs):
	for kwarg in kwargs:
		print(kwarg," ",kwargs[kwarg])
indeterminados_nombre(n=5,c="Hola",l=[1,2,3,4,5])
	
````
OUT:
````bash
n 5
c Hola
l [ 1, 2, 3, 4, 5]
````

## Por posicion y nombre a la vez
Si queremos aceptar ambos tipos de parametros simultaneamente, entonces debemos crear ambas colecciones dinamicas:
````python
def super_funcion(*args, **kwargs):
	t=0
	for arg in args:
		t += arg
	print("Sumatorio indeterminado es",t)
	for kwarg in kwargs:
		print(kwarg," ",kwargs[kwarg])
super_funcion(10,50,-1,1.56,10,20,300,nombre="Yael", edad=21)
````
OUT:
````bash
Sumaterio indeterminado es 390.56
nombre Yael
edad 21
````

[[Diccionarios]]