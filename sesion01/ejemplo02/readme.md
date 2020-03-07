## Variables y tipos de datos

Una variable nos permite almacenar datos y usarlos a lo largo de un programa mediante el nombre que le dimos a dicha variable. Para crear una variable, basta con asignarle un nombre, que comience con una letra. Una variable puede almacenar números, texto u otros rangos de valores a los cuales llamamos *tipos*.

__Python__ es un lenguaje que usa *tipificado dinámico*, esto quiere decir que las variables no están cazadas con un tipo y pueden almacenar cualquier de estos.

![imagen](https://i.shelterness.com/how-to-label-things-in-your-home-014-500x333.jpg)

En Python se tienen distintos tipos de datos.

### 1. Booleanos (`bool`)

Las constantes verdadero y falso representadas con `True` y `False` respectivamente.

```python
In [1]: True
Out[1]: True

In [2]: False
Out[2]: False
```

### 2. Números enteros (`int`, `long`)

```python
In [1]: 1
Out[1]: 1

In [2]: -2
Out[2]: -2

In [3]: 1729
Out[3]: 1729
```

### 3. Números de punto flotante (`float`, `double`)

Es decir números fraccionarios (con punto decimal).

```python
In [1]: 18.3
Out[1]: 18.3

In [2]: 14.5
Out[2]: 14.5
```

### 4. Números complejos (`complex`)

Con una parte real y una imaginaria representada por `j`.

```python
In [1]: 2.1 + 7.8j
Out[1]: (2.1+7.8j)
```

### 5. Cadenas (`str`)

Es texto encerrado entre comillas simples `'` o dobles `"`. Dentro de las comillas se mueden añadir caracteres especiales escapándolos con `\` como `\n` para saltos de línea o `\t` para tabuladores

```python
In [1]: 'cadena'
Out[1]: 'cadena'

In [2]: "cadena"
Out[2]: "cadena"
```

### 6. Variables

Para declarar variables, basta escribir sun nombre, seguidas de un símbolo `=` y el valor asociado a estas, pudiendo ser alguno de los tipos anteriores.

```python
In [1]: a = 1729

In [2]: 
```

Para conocer el tipo de una variable, podemos usar la función `type`. Más adelante definimos qué es una función.

```python
In [1]: a = 1729

In [2]: type(a)
Out[2]: int
```

### 7. Operaciones aritméticas

| Operador | Descripción     |
| -------- | ----------------|
| `+`      | Suma            |
| `-`      | Negación        |
| `*`      | Producto        |
| `**`     | Exponente       |
| `/`      | División        |
| `//`     | División entera |
| `%`      | Módulo          |

Veamos algunos ejemplos:

```python
In [1]: a = 3

In [2]: b = 2

In [3]: a + b
Out[3]: 5

In [4]: a - b
Out[4]: 1

In [5]: a * b
Out[5]: 6

In [6]: a ** b
Out[6]: 9

In [7]: a / b
Out[7]: 1.5

In [8]: a // b
Out[8]: 1

In [9]: a % b
Out[9]: 1
```

[Volver](../readme.md)
