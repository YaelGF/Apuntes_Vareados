# La funcion range()

Sirve para generara una lista de numeros que podemos recorrer facilmente, pero no ocupa memoria porque se interpreta sobre la marcha:

```python
for i in range(10)
    print(i)
```
OUT:
```bash
0
1
2
3
4
5
6
7
8
9
```

```python
range(10)
```
OUT:
```bash
range(0,10)
```

Si queremos conseguir la lista literal podemos transformar el range a una lista:
```python
list(range(10))
```
OUT:
```bash
0
1
2
3
4
5
6
7
8
9
```
