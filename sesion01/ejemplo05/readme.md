## Estruturas de control

### Estructura de decisión `if`

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

### While
Ejecuta una pieza de código, en ciclos, hasta que la condición indicada se deje de cumplir.
`while_5.py`
```
In [5]: while n<5: 
   ...:     print("Numero {}".format(n)) 
   ...:     n = n + 1 
   ...:                                                                                                                                                                                      
Numero 0
Numero 1
Numero 2
Numero 3
Numero 4

`for_5.py`
```
### For
Itera sobre cada uno de los elementos que se le indiquen.
```
In [7]: for i in range(5): 
   ...:     print("Numero {}".format(i)) 
   ...:      
                                                                                                                                                        
Numero 0
Numero 1
Numero 2
Numero 3
Numero 4

```
#### Ejemplo: par_non.py
De una lista de 10 numeros, imprimir en pantalla par o non, dependiendo de si son divisibles entre 2 o no.

```python
In [8]: for i in range(11): 
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
