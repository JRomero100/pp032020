## Estruturas de control

### 1. Estructura de decisión `if`

Permite cambiar el flujo de ejecución de un programa o *script* al tomar decisiones con base en lo que se conoce como condición. La estructura generalde un if es la siguiente:

```python
if condición1:
   ...
elif condición2:
   ...
else:
   ...
```

La condición que recibe el `if` debe ser un valor booleano, en ese sentido podemos usar los operadores lógicos o lo que se conoce como *operadores relacionales* para números:

| Operador | Significado       |
| -------- | ----------------- |
| `<`      | Menor que         |
| `<=`     | Menor o igual que |
| `>`      | Mayor que         |
| `>=`     | Mayor o igual que |
| `==`     | Igual que         |
| `!=`     | Distinto de       |

De esta forma si se cumple la condición, evaluamos el código que se encuentra inmediatamente después indentado. Después con `elif` podemos probar otra condición en caso de no cumplirse la anterior, esta condición puede omitirse y puede haber más de un `elif` a la vez. Si ninguna condición se cumple, se ejecuta el cuerpo del `else`. Por ejemplo:

*Script*: `positivo_negativo.py`

```python
numero = input('Introduce un número: ')

if int(numero) == 0:
   print("El número es cero.")
elif int(numero) > 0:
   print("El número es positivo.")
else:
   print("El número es negativo.")
```

*Ejemplo de ejecución*

```bash
Introduce un número: 0
El número es cero.
```

### 2. Estructura de repetición `while`

Ejecuta un fragmento de código en repetidas ocasiones mientras la condición especificada se cumpla. La sintaxis general de un `while` es:

```python
while condición:
   ...
```

Por ejemplo, queremos imprimir los primeros 5 números naturales.

```python
In [1]: n = 0
In [2]: while n < 5: 
   ...:     print("Número {}".format(n))
   ...:     n = n + 1

Numero 0
Numero 1
Numero 2
Numero 3
Numero 4
```

### 3. Estructura de repetición `for`

Al igual que `while` realiza iteraciones, sin embargo en lugar de recibir una condición utiliza un conjunto de elementos, sobre los cuales iterar. La forma más sencilla de usar for es con la función `range` que genera un conjunto de elementos del 0 al número indicado.

La estructura de un `for` es:

```python
for i in elementos:
   ...
```

Por ejemplo:

```python
In [1]: for i in range(5): 
   ...:     print("Número {}".format(i)) 
   ...:
                               
Numero 0
Numero 1
Numero 2
Numero 3
Numero 4
```
### Ejemplo: Pares y nones
De una lista de 10 numeros, imprimir en pantalla par o non, dependiendo de si son divisibles entre 2 o no.

```python
In [1]: for i in range(11): 
   ...:     if i % 2 == 0: 
   ...:         print("Par") 
   ...:     else: 
   ...:         print("Non") 
   ...:   
   
Par
Non
Par
Non
Par
Non
Par
Non
Par
Non
```

[Volver](../readme.md)
