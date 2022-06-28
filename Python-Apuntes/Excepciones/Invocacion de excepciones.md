# Invocación de excepciones
En algunas ocasiones quizá nos interese llamar un error manualmente, ya que un print común no es muy elegante:
```python
def mi_funcion(algo=None):
	if algo is None:
		print("Error! No se permite un valor nulo (con un print)")
mi_funcion()
```
OUT:
```bash
Error! No se permite un valor nulo (con un print)
```
## La instrucción raise
Gracias a raise podemos lanzar un error manual  pasándole el identificador. Luego simplemente podemos añadir un except para tratar esta excepción que hemos lanzado:
```python
def mi_funcion(algo=None):
	try:
		if algo is None:
			raise ValueError()
	except ValueError:
		print("Error! No se permite un valor nulo (desde la excepción)")
mi_funcion()
```
OUT:
```bash
Error! No se permite un valor nulo (desde la excepción)
```