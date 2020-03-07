## Ejemplo 01

### Estructuras de datos

### Listas

<img src="https://media.giphy.com/media/B7o99rIuystY4/giphy.gif" align="right" width="300" height="300">

Son estructuras de datos mutables, el acceso a sus elementos puede lograrse mediante un índice. Pueden contener cualquier tipo de dato, y no necesariamente deben ser del mismo tipo, es decir son *heterogéneas*.

```python 
In [1]: l1 = []

In [2]: l2 = list()

In [3]: l1 == l2
Out[3]: True

In [4]: l2 = [1, 2, 3, 4, 5]

In [5]: l3 = [1.2, 3.5, 6.5, 0.7, 4.6]

In [6: l4 = ["a", "agg", "Hola Lista"]

In [7]: l5 = [10, 5.0, "Doscientos"]

In [8]: type(l5)
Out[8]: list
```

Podemos generar un *script* que genere e imprima una lista con números enteros, comnezando con 0, y finalizando con un número entero definido por el usuario.

```python
n = input("Tamaño de la lista: ")

if not n.isdigit():
    print("Número invalido")

else:
    n = int(n)

    lista = list(range(n))
    for i in lista:
        print(i)
```        

```bash
$ python3 lista-de-enteros.py
Tamaño de la lista: 10
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

Este script, que parece inofensivo a simple vista, ¡puede colapsar tu equipo! Si la lista es demasiado grande, puede llenar la memoria RAM.

[Volver](../readme.md)
