## Cadenas

Como dijimos antes, las cadenas son texto asignado a una variable. Deben estar encerrados en comillas simples o comillas dobles. Como ya vimos, en el reto anterior, también podemos hacer ciertas operaciones con ellas. Por ejemplo:

```python
In [1]: d = "Hola mundo"

In [2]: type(d)
Out[2]: str

In [3]: e = 'Saludos'

In [4]: f = ""What's your name?""

In [5]: "Hola" * 5
Out[5]: 'HolaHolaHolaHolaHola'

In [6]: "Hola" + " Mundo"
Out[6]: 'Hola Mundo'

```

__Python__ no convierte automáticamente tipos de datos, por lo cual, no podemos hacer una suma con un numero entero y una cadena. Esto lo hace un lenguaje *de tipo seguro*. Podemos convertir datos utilizando el nombre del tipo de dato, y el dato entre paréntesis, como lo hicimos en el reto pasado.

```python
In [1]: 5 + "5"
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-18-b265071c056c> in <module>
----> 1 5 + "5"

TypeError: unsupported operand type(s) for +: 'int' and 'str'

In [2]: 5 + int("5")
Out[2]: 10

In [3]: str(5) + "5"
Out[3]: '55'

```

Podemos usar variables en una cadena, mediante especificadores de formato usando la función `format()`. Ésta convierte los datos a cadenas, para posteriormente, imprimirlos en pantalla. Tabién podemos pedir datos al usuario desde teclado usando `input()`.

*Script:* [`formato.py`](format.py)

```python
nombre = input('¿Cuál es tu nombre?: ')
edad   = input('¿Cuál es tu edad?: ')

print("Hola, {} tu edad es {}".format(nombre,edad))
```

*Ejemplo de ejecución:*

```python
In [1]: run format.py
¿Cuál es tu nombre?: Dady Yankee
¿Cuál es tu edad?: 18
Hola, Dady Yankee tu edad es 18

In [2]:
```

![image](https://media1.tenor.com/images/1a04a3819aeff6c2f2cdfe99028cf504/tenor.gif?itemid=5168072)

Ahora sabes cómo formatear cadenas y Daddy Yankee está orgulloso de ti. La función `format` tiene una gran cantidad de configuraciones para insertar nuestros datos en una cadena. Podemos conocer más a fondo su funcionamiento en la página https://pyformat.info

[Volver](../readme.md)
