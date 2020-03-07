## Ejemplo 02: Operaciones con listas

Las listas pueden modificar, agregar y eliminar sus elementos. También pueden hacerse operaciones con ellas. Algunas de estas operaciones son:

| Operación | Descripción                              |
| --------- | ---------------------------------------- |
| `append`  | Agrega un elemento al final de la lista  |
| `insert`  | Inserta elementos en el índice dado      |
| `+`       | Concatena dos listas                     |
| `join`    | Convierte listas a cadenas               |

Además, podemos usar la biblioteca `random` obtener valores al azar o desordenar una lista aleatoriamente. Usando corchetes después de la lista e indicando un número se obtiene el valor en la posición indicada.

```python
In [1]: l1 = ["a", "b", "c"]

In [2]: l1.append("d")

In [3]: l1
Out[3]: ['a', 'b', 'c', 'd']

In [4]: l2 = [ 2, 3, 4, 5]

In [5]: l2.insert(0, 1)  # Indice, valor

In [6]: l2
Out[6]: [1, 2, 3, 4, 5]

In [7]: l1 + l2
Out[7]: ['a', 'b', 'c', 'd', 1, 2, 3, 4, 5]

In [8]: "".join(l1)
Out[8]: 'abcd'

In [9]: ", ".join(l1)
Out[9]: 'a, b, c, d'

In [10]: import random

In [11]: random.choice([1,2,3,4,5,6])
Out[11]: 5 # Elemento al azar

In [12]: l3 = list("abc123")

In [13]: random.shuffle(l3) # Desordena la lista

In [14]: l3
Out[14]: ['a', '3', 'c', 'b', '2', '1']

In [15]: lista_de_listas = [ [0,1,2], [3,4,5], [6,7,8] ]

In [16]: lista_de_listas[1][0]
Out[16]: 3

In [17]: lista_de_listas[2]
Out[17]: [6, 7, 8]
```

Veamos, por ejemplo, cómo generar clasves aleatorios usando estos conceptos. Estas claves tienen al menos 1 mayúscula, una minúscula y un dígito, con longitud `m`. `n` y `m` serán solicitados al usuario, este úlutmo con un valor de 8 por defecto.

*Script:* [`genera-claves.py`](genera-claves.py)

```python
import random

n = input("Número de claves a generar: ")

if not n.isdigit():
    print("Valor inválido")
    quit()
else:
    n = int(n)

m = input("Longitud de claves (8): ")

if m == "":
    m = 8
elif m.isdigit():
    m = int(m)
else:
    print("Valor inválido")
    quit()

# Listas de elementos para generar claves
digits = "1234567890"
minus = "qwertyuiopasdfghjklzxcvbnm"
mayus = minus.upper()

for i in range(n):
    # Obtener minimo 1 de cada elemento
    digito = random.choices(digits)
    minuscula = random.choices(minus)
    mayuscula = random.choices(mayus)
    # El resto seran elementos al azar de las 3 listas
    resto = random.choices(digits + minus + mayus, k=m-3)
    contrasena = digito + minuscula + mayuscula + resto
    random.shuffle(contrasena) # Mezclar los elementos para cambiar su orden
    contrasena = "".join(contrasena) # Convertirla a string
    print(contrasena)
```

``` bash
$ python3 genera-claves.py 
Número de claves a generar: 3
Longitud de claves (8): 
wDxIg9BJ
8U3lNI2E
0QiZqQRY
```

[Volver](../readme.md)
