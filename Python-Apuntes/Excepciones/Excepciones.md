# Bloque else en excepciones
[Mas información](https://docs.python.org/3/library/exceptions.html#base-classes)
Es posible encadenar un bloque else despues del except para comprobar el caso en que todo funcione correctamente(no se ejecuta la excepcion).
El bloque else es un buen momento para romper la iteracion con break si todo funciona correctamente:
```python
while(True):
	try:
		n=float(input("Introduce un numero: "))
		m=4
		print("{}/{}={}".format(n,m,n/m))
	except:
		print("Ha ocurrido un error, introduce bien el número")
	else:
		print("Todo ha funcionado correctamente")
		break
```
OUT:
```bash
Introduce un número: Yael
Ha ocurrido un error, introduce bien el número Introduce un número: 3 
3.0/4=0.75 
Todo ha funcionado correctamente
```
# Bloque finally
Por ultimo es posible utilizar un bloque finally que se ejecute al final del codigo, ocurra o no ocurra un error:
```python
while(True):
	try:
		n=float(input("Introduce un numero: "))
		m=4
		print("{}/{}={}".format(n,m,n/m))
	except:
		print("Ha ocurrido un error, introduce bien el número")
	else:
		print("Todo ha funcionado correctamente")
		break
	finally:
		print("Fin du la iteración")# Siempre se ejecuta
```
OUT:
```bash
Introduce un número: aaa 
Ha ocurrido un error, introduce bien el número Fin de la iteración 
Introduce un número: 10 
10.0/4=2.5 
Todo ha funcionado correctamente 
Fin de la iteración
```

