# Rutas

Para evitar los caracteres especiales, debemos indicar que es una cadena cruda(raw)

```python
#String normal
print("C:\nombre\directorio")
#String cruda
print(r"C:\nombre\directorio") #r => raw(cruda)
```

OUT:
```bash
#Salida 1
C:
ombre\directorio
#Salida 2
C:\nombre\directorio
```
# Slicing

El slicing es una capacidad de las cadenas que devuelven un subconjunto o subcadena utilizando indices [inicio:fin:salto]

---------------
* El primer indice indica donde empezar la subcadena(se incluye el caracter)
* El segundo indice indica donde acabbba la subcadena (se excluye el caracter)
* El tercer indice indica cada cuantos caracteres salta

```python
palabra = "Python"
print(palabra[0:-1:2])
```

OUT:
```bash
Pto
```
