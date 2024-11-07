**Ordenando elementos**
```
nombres.sort()
print(nombres)
```
---
**Contando elementos**
```
for nombre in nombres:
    if nombre.startswith("A"):
        contador += 1
print(contandor)
```
---
**Buscar un elementos**
```
cadena = input("Inserte una cadena")
if cadena in nombres:
    posicion = nombres.index(cadena)
    print(cadena + " existe en la posicion " + str(posicion))
else:
    print(cadena + " no existe")
```
---
**Primeros elementos**
```
cadena = input("Dime tu nombre")
posicion = nombres.index(cadena)
```
---
**Obtener número de nombres de una longitud**
```
cadena = int(input("Inserte una cadena"))
total = 0;
for nombre in nombres:
    if len(nombre) == cadena:
        total += 1
print("Hemos encontrado: " + str(total) + " resultados")
```
---
**Nombres cortos**
```
for nombre in nombres:
    if len(nombre) <= 4:
        print(nombre)
```
---
**Número de vocales**
```
a = 0
e = 0
i = 0
o = 0
u = 0
for nombre in nombres:
    for caracter in nombre:
        if(caracter == 'a'):
            a += 1
        elif(caracter == 'e'):
            e += 1
        elif(caracter == 'i'):
            i += 1
        elif(caracter == 'o'):
            o += 1
        elif(caracter == 'u'):
            u += 1
print("Total de a " + str(a))
print("Total de e " + str(e))
print("Total de i " + str(i))
print("Total de o " + str(o))
print("Total de u " + str(u))
```
---
**Número de letras**
```
from collections import Counter
nombres = ["Alejandro", "María", "Javier", "Lucía", "Carlos", "Sofía", "Miguel", "Ana", "Manuel", "Isabel", "Pedro", "Carmen", "Jorge", "Elena", "Juan", "Laura", "Antonio", "Patricia", "David", "Claudia", "Francisco", "Marta", "Sergio", "Teresa", "Luis", "Raquel", "Andrés", "Paula", "Daniel", "Verónica", "Fernando", "Sara", "Pablo", "Irene", "Álvaro", "Natalia", "Hugo", "Eva", "Diego", "Cristina", "Jesús", "Rosa", "Roberto", "Alicia", "Ángel", "Beatriz", "Ricardo", "Julia", "Adrián", "Silvia", "Alberto", "Victoria", "Raúl", "Pilar", "Ramón", "Lidia", "Óscar", "Ariadna", "Gonzalo", "Mónica", "Rubén", "Esther", "Santiago", "Nuria", "Iván", "Ainhoa", "Eduardo", "Berta", "Marcos", "Noelia", "Enrique", "Elisa", "Emilio", "Fátima", "Vicente", "Gabriela", "Mario", "Olga", "Rafael", "Lorena", "Mariano", "Cristina", "Eugenio", "Mercedes", "Félix", "Amparo", "Sebastián", "Rocío", "Alfredo", "Esperanza", "Álex", "Celia", "Héctor", "Andrea", "Tomás", "Inés", "Marcelo", "Gloria", "Marina", "Belén", "Valentín", "Miriam", "Guillermo", "Ángela", "Joaquín", "Gemma", "Fabián", "Daniela", "Víctor", "Dolores", "Marcos", "Tamara", "Braulio", "Lourdes", "Federico", "Gema", "Julián", "Nicolás", "Leandro", "Manuela", "Agustín", "Elsa", "Julio", "Consuelo", "Ismael", "Alejandra", "Joaquín", "Milagros", "Gregorio", "Inmaculada", "Salvador", "Carla", "Esteban", "Carolina", "Fausto", "Emilia", "Alfonso", "Amalia", "Baltasar", "Adela", "Humberto", "Blanca", "Aníbal", "Araceli", "César", "Candela"]

nombresLimpia = "".join(nombres).lower()

contador = Counter(caracter for caracter in nombresLimpia if caracter.isalpha())

for letra, conteo in contador.items():
    print(str(letra) + " : " + str(conteo))
```
---
**Sumar elementos de una lista**
```
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9]
total = 0
for numero in numeros:
	total += numero
print(total)
```
---
**Contar elementos específicos**
```
nombres = ["Alejandro", "María", "Javier", "Lucía", "Carlos"]

cadena = input("Inserte una cadena")

contador = nombres.count(cadena)

print("La palabra " + str(cadena) + " aparece " + str(contador) + " veces")
```
---
**Eliminar duplicados**
```
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 2, 3, 4, 5, 6, 7, 8, 9]
for numero in numeros:
    if numeros.count(numero) > 1:
        numeros.remove(numero)
print(numeros)
```
---
**Máximo y mínimo**
```
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9]
minimo = min(numeros)
maximo = max(numeros)
print("Valor minimo: " + str(minimo))
print("Valor maximo: " + str(maximo))
```
---