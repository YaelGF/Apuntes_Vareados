# Los conjuntos
Son colecciones desordenadas de elementos unicos utilizados para hacer pruebas depertenecia a grupos y eliminacion de elementos duplicados.

```python
conjunto = set()
conjunto = {1,2,3}
conjunto.add(4)

print(conjunto)
```
OUT:
```bash
{1,2,3,4}
```

## Los conjuntos son Desordenados
Se dice que son desordinados porque gestionan automaticamente la posicion de sus elementos, en lugar de conservarlos en la posicion que nosotros los añadimos.

```python
conjunto.add("H")
conjunto.add("A")
conjunto.add("Z")

print(conjunto)
```
OUT:
```bash
{1,2,3,4,'H','Z','A'}
```

## Auto-eliminacion de elementos duplicados

```python
test = {'Hector','Hector','Hector'}

print(test)
```
OUT:
```bash
{'Hector'}
```

## Cast de listas a conjunto y viceversa
Es muy util transformar listas a conjuntos para borrar los elementos duplicados automaticamente

```python
l = [1,2,3,3,2,1]

c = set(l)

l = list(c)

print(l)
```
OUT:
```bash
[1,2,3]
```

```python
l = list( set( l ) )
```
OUT:
```bash
[1,2,3]
```
