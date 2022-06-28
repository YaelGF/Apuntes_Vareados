# Las colas 
Son colecciones de elementos ordenados que unicamente permiten dos acciones:

* Añadir un elemento a la cola
* Sacar un elemento de la cola

La peculiaridad es que el primer elemento en entrar es el primero en salir. En ingles se conocen como estructuras FIFO (First In First Out)

## Debemos importar la coleccion deque manualmente para creal una cola

```python
from collections import deque

cola = deque(["Hector","Juan","Miguel"])
```

## Popleft()en lugar de pop()
A la hora de sacar los elementos utilizaremos el metodo popleft()para extraerlos por la parte izquierda (el principio de la cola). Al igual que antes, debemos asegurarnos de almacenar los elementos al sacarlos o los perderemos.

```python
print(cola.popleft())
```

OUT:
```bash
Hector
```
