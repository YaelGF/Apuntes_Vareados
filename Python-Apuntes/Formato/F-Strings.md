# F-Strings
Desde python 3,6 encontramos una nueva funcionalidad que simplificar el formateo gracias a la interpretacion de cadenas.

En lugar de poner ".format()" ponemos esto:
```python
nombre = "Yael"
cadena = "Hola {}".format(nombre)
print(cadena)
```
OUT:
```bash
Hola Yael
```
## Podemos indicar que la cadena está formateada añadiendo `f"{}"` delante y 

*   Elemento de la lista
*   Elemento de la lista

pasando directamente las variables o datos interpretados:

```python
nombre = "Yael"
cadena = f"Hola {nombre}"
print(cadena)
```
OUT:
````bash
Hola Yael
````
## Contenido interpretado
```python
a, b = 10, 5
print(f"La suma de {a} y {b} es {a+b}")
```
OUT:
```bash
La suma de 10 y 5 es 15
```

````python
def func():
	return "Yael"

print(f"Hola {func()}!")
````
OUT:
````bash
Hola Yael!
````

````python
numero = {"uno":1,"dos":2,"tres":3}

print(f"El numero dos es {numero['dos']}")
````
OUT:
````bash
El numero dos es 2
````
## Formateos avanzados

### Alineamientos
````python
texto = "Hola mundo"
````
#### A la izquierda por 40 caracteres
```python
print(f"{texto:40}")
```
OUT
```bash
Hola mundo
```

#### A la derecha por 40 caracteres
```python
print(f"{texto:>40}")
```
OUT
```bash
                              Hola mundo
```
#### Al centro por 40 caracteres
```python
print(f"{texto:^40}")
```
OUT
```bash
               Hola mundo               
```
### Truncamiento
```python
print(f"{texto:.4}")
```
OUT
```bash
Hola
```
### Truncamiento con variables
```python
limite = 4
print(f"{texto:.{limite}}")
```
OUT
```bash
Hola
```
### Alineamiento con truncamiento
```python
print(f"{texto:>30.4}")
print(f"{texto:<30.4}")
print(f"{texto:^30.4}")
```
OUT
```bash
                          hola
hola
             hola             
```
### Alineamiento con truncamiento y variables
```python
limite = 4
longitud = 30

print(f"{texto:>{longitud}.{limite}}")
print(f"{texto:<{longitud}.{limite}}")
print(f"{texto:^{longitud}.{limite}}")
```
OUT
```bash
                          hola
hola
             hola             
```
### Formateo de numeros enteros, rellenados con espacios
```python
print(f"{1:6d}")
print(f"{10:6d}")
print(f"{100:6d}")
print(f"{1000:6d}")
print(f"{10000:6d}")
print(f"{100000:6d}")
```
OUT
```bash
     1
    10
   100
  1000
  1000
 10000
100000   
```
### Formateo de numeros enteros, rellenados con ceros
```python
print(f"{1:06d}")
print(f"{10:06d}")
print(f"{100:06d}")
print(f"{1000:06d}")
print(f"{10000:06d}")
print(f"{100000:06d}")
```
OUT
```bash
000001
000010
000100
001000
010000
100000          
```
### Formateo de numeros flotantes, rellenados con espacios
```python
print(f"{3.1415926:7.3f}")
print(f"{153.21:7.3f}")
```
OUT
```bash
  3.142 
153.210            
```
### Formateo de numeros flotantes, rellenados con ceros
```python
print(f"{3.1415926:09.4f}")
print(f"{153.21:09.4f}")
```
OUT
```bash
0003.1416
0153.2100
```
### Formateo de numeros con variables
```python
numero = 3.1415926
longitud = 21 # 1 para el decimal
decimales = 10

  

print(f"{numero:0{longitud}.{decimales}f}")
```
OUT
```bash
0000000003.1415926000          
```
