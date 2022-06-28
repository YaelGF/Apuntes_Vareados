# Expresiones anidadas 
Se pueden solucionar empleando las reglas de precedencia:

* Primero los parentesis, porque tienen prioridad
* Segundo, las expresiones aritmeticas por sus propias reglas
* Tercero, las expresiones relacionales
* Cuarto, las expresiones logicas

```python
a = 10
b = 5

print(a * b - 2**b," es mayor o igual a 20?")

print((a%b)," no es  diferente a 0?")

print( a*b - 2**b >= 20 and not (a % b ) != 0)
```

OUT:

```bash
#Salida 1
18  es mayor o igual a 20?
#Salida 2
0  no es  diferente a 0?
#Salida 3
False
```
