# El metodo .items()
Nos facilita la lectura en clave y valor de los elementos porque devuelven ambos valores en cada interacion automaticamente:

```python
edades = {"Yael":20,"Arturo":21,"Adrian":26}

for c,v in edades.items():
    print(c,v)
```
OUT:
```bash
Yael 20
Arturo 21
Adrian 26
``` 

Otra forma de declarar dicionarios puede ser:

```python
edades = dict(Yael=20,Arturo=21,Adrian=26)
```
