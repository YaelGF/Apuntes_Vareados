# El metodo .format()
Es una funcionalidad de las cadenas de texto que nos permite formatear informacion en una cadena (varibles o valores literahles) comodamente utilizando referenciados:
```python
print("Un texto '{}' y un numero '{}'".format("Hola",3))
```
OUT:
```bash
Un texto 'Hola' y un numero '3'
```

Tambien podemos referenciar a partir de la posicion de los valores utilizando indices:
```python
print("Un texto '{1}' y un numero '{0}'".format("Hola",3))
```
OUT:
```bash
Un texto '3' y un numero 'Hola'
```

O podemos utilizar identificador con una clave y luego pasarlas en el format:

```python
print("Un texto '{str}' y un numero '{n}'".format(str="Hola",n=3))
```
OUT:
```bash
Un texto 'Hola' y un numero '3'
```

## Formateo Avanzado

### Alineamiento a la derecha en 30 caracteres

```python
print("{:>30}".format("palabra"))
```
OUT:
```bash
                       palabra
```

### Alineamiento a la izquierda en 30 caracteres

```python
print("{:30}".format("palabra"))
```
OUT:
```bash
palabra                       
```

### Alineamiento al centro en 30 caracteres

```python
print("{:^30}".format("palabra"))
```
OUT:
```bash
           palabra            
```

### Truncamiento a 3 caracteres

```python
print("{:.3}".format("palabra"))
```
OUT:
```bash
pal
```

### Alineamiento a la derecha en 30 caracteres con truncamiento de 3

```python
print( "{:>30.3}".format("palabra") )
```
OUT:
```bash
                           pal
```

### Formateo de numeros enteros, rellenados por espacios

```python
print("{:4d}".format(10))
print("{:4d}".format(100))
print("{:4d}".format(1000))
```
OUT:
```bash
  10
 100
1000
```

### Formateo de numeros enteros, rellenados con ceros

```python
print("{:7.3f}".format(3.1415926))
print("{:7.3f}".format(153.21))
```
OUT:
```bash
  3.142
153.210
```

### Formateo de numeros flontantes, rellenados con espacios

```python
print("Un texto '{str}' y un numero '{n}'".format(str="Hola",n=3))
```
OUT:
```bash
Un texto 'Hola' y un numero '3'
```

### Formateo de numeros flontantes, rellenados con ceros

```python
print("{:07.3f}".format(3.1415926))
print("{:07.3f}".format(153.21))
```
OUT:
```bash
003.142
153.210
```

