## Operadores lógicos

Al igual que los números, los valores booleanos tienen un conjunto de operaciones que permiten obtener un cierto valor de verdad. Éstas reciben el nombre de *operadores lógicos* y se definen a continuación.

Para mostrar el comportamiento de estos operadores, se usa lo que se conoce como *tabla de verdad*.

### 1. Operación `not`

Niega un valor de verdad. Esto es, si el valor booleano es `False` se cambia por `True` y viceversa.  Su tabla de verdad es la siguiente.

| `p`     | `not p` |
| ------- | ------- |
| `True`  | `False` |
| `False` | `True`  |

```python
In [1]: not True
Out[1]: False

In [2]: not False
Out[2]: True
```

### 2. Operación `and`

Verifica que dos valores sean verdaderos, es decir, que dos proposiciones se cumplan. Una proposición es un enunciado que puede ser verdadero o falso. Su tabla de verdad es la siguiente.

| `p`     | `q`     | `p and q` |
|---------|---------|-----------|
| `False` | `False` | `False`   |
| `False` | `True`  | `False`   |
| `True`  | `False` | `False`   |
| `True`  | `True`  | `True`    |

```python
In [1]: True and True
Out[1]: True

In [2]: True and False
Out[2]: False
```

### 3. Operación `or`

Verifica alguno de los dos valores sean verdadero, es decir, que alguna de las dos proposiciones se cumplan. Su tabla de verdad es la siguiente.

| `p`     | `q`     | `p or q` |
|---------|---------|-----------|
| `False` | `False` | `False`   |
| `False` | `True`  | `True`   |
| `True`  | `False` | `True`   |
| `True`  | `True`  | `True`    |

```python
In [1]: True or True
Out[1]: True

In [2]: False or False
Out[2]: False
```

[Volver](../readme.md)
