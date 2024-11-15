**Filtrado de una lista de números**
```
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
def funcionNumeros(x):
    return x % 2 == 0 
listaResuelta = list(filter(funcionNumeros, numeros))
print(listaResuelta)
```
---
**Mapeo de temperaturas**
```
celsius = [0, 20, 37, 100]
fahrenheit = list(map(lambda x: (x * 9/5) + 32, celsius))
print(fahrenheit)
```
---
**Suma acumulativa**
```
from functools import reduce
numeros = [1, 2, 3, 4, 5]
suma = reduce(lambda acc, val: acc + val, numeros)
print(suma)
```
---
**Palabras con cierta longitud**
```
palabras = ["perro", "gato", "elefante", "oso", "jirafa"]
def funcionAnimales(x):
    return len(x) > 5
listaAnimales = list(filter(funcionAnimales, palabras))
def listaMayuscula(y):
    return y.upper()
lisaUpper = list(map(listaMayuscula, listaAnimales))
print(lisaUpper)
```
---
**Multiplicación de pares**
```
from functools import reduce
numeros = [1, 2, 3, 4, 5, 6]
numerosPares = filter(lambda x: x % 2 == 0, numeros)
resultadoPares = reduce(lambda x, y: x * y, numerosPares)
print(resultadoPares)
```
---
**Combinar operaciones en listas anidadas**
```
from functools import reduce
numeros = [[-3, 2, 7], [10, -5, 3], [0, 8, -2]]
guardarPositivos = map(lambda lista: list(filter(lambda y: y > 0, lista)), numeros)
todosLosPositivos = [numero for lista in guardarPositivos for number in lista]
total = sum(todosLosPositivos)
print(total)
```
---