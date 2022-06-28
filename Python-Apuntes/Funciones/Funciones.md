# Funciones
## La instruccion global
Para poder modificar una variable externa en la funcion, debemos indicar que es global de la siguiente forma:

````python
def test():
	global o #variable que hace referencia a la o externa
	o = 5
	print(o)
	
test()
o = 10
test()
print(o)
````
OUT:
````bash
5
5
5
````

## Parametros por defecto
Para solicionar el error que al llamar una funcion que tiene definidos unos parametros, si no pasamos los argumentos correctamente provocara un error; podemos asignar unos valores por defecto nulos a los parametros, y de esta forma podriamos hacer una comprobacion antes de ejecutar el codigo de la funcion:

````python
def resta(a=None, b=None):
	if a == None or b == None:
		print("Error, debes enviar dos números a la función")
	return a-b
resta()
````
OUT:
````bash
Error, debes enviar dos números a la función
````

## Paso por valor y paso por referencia
* **Paso por valor**: Se crea una copia local de la variable dentro de la funcion.
* **Paso por referencia**: Se maneja directamente  la variable, los cambios realizados dentro le afectaran tambien fuera.
Tradicionalmente, los tipos simples  se pasan automaticamente por valor y los compuestos por referencia.
* **Simples**: Enteros, Flotantes, Cadenas, Lógicos...
* **Compuestos** : Listas, Diccionarions, Conjuntos...

### Ejemplo del paso por valor
````python
def doblar_valor(numero):
	numero *= 2
n = 10
doblar_valor(n)
print(n)
````
OUT:
````bash
10
````
### Ejemplo del paso por referencia
````python
def doblar_valores(numeros):
	for i,n in enumerate(numeros):
		numeros[i] *= 2
ns = [10,50,100]
doblar_valores(ns)
print(ns)
````
OUT:
````bash
[ 20, 100, 200 ]
````
nota:[[Generador-Indices]]

### Trucos
#### Para modificar los tipos simples podemos devolverlos modificados y reasignarlos:
````python
def doblar_valor(numero):
	return numero *2
n = 10
n = doblar_valor(n)
print(n)
````
OUT:
````bash
20
````
#### Y en el caso de los tipos compuestos, podemos evitar la modificacion enviando una copia:
````python
def doblar_valores(numeros):
	for i,n in enumerate(numeros):
		numeros[i] *= 2
ns = [10,50,100]
doblar_valores(ns[:]) # Una copia al vuelo de una lista con [:]
print(ns)
````
OUT:
````bash
 [ 10, 50, 100 ]
````

[[Argumentos y parametros indeterminados]]