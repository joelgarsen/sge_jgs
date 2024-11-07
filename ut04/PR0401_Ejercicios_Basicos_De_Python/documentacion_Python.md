**1. Lectura de un número válido**
```
numero = input("Introduce un numero")
while(not numero.isdigit()):
    print("Error")
    numero = input("Introduce un numero")
print(numero)
```
---
**2. Tabla de multiplicar**
```
numero = input("Introduce un numero")
while(not numero.isdigit()):
    print("Error")
    numero = input("Introduce un numero")
print(numero)
```
---
**3. Triángulo de asteriscos**
```
numero = int(input("Introduce numero"))
for asteriscos in range(numero):
    caracter = ""
    for asterisco in range(asteriscos+1):
       caracter += "*"
    print(caracter)
```
---
**4. Pirámide de asteriscos**
```
base = int(input("Introduce un numero impar"))
while(base % 2 == 0):
    print("Error")
    base = int(input("Introduce un numero impar"))
for i in range(i, base+1,2):
    espacios = (base-i) / 2
    print(" " * int(espacios) + "*" * i)
```
---
**5. Número mayor y menor**
```
for numero in range(5)
    numeroAlto = 0;
    NumeroBajo = 0;
    numero = int(input("Introduce numero"))
    if(numero < numeroBajo):
        numero = numeroBajo
    elif(numero > numero Alto):
        numero = numeroAlto

print("El numero mayor es" + numeroAlto + "y el menor" + numeroMenor)
```
---
**6. Conversión de unidades**
```
numero = int(input("Introduce un numero"))
medida = input("Introduce una medida")
medidaPasar = input("Introduce la medida a la que deseas pasarlo")
match(medida)
    case "mm":
        if (medidaPasar == "mm"):
        numero = numero * 1
        elif (medidaPasar == "m"):
        numero = numero / 1000
        elif(medidaPasar = "km"):
        numero = numero / 1000000

    case "m":
        if (medidaPasar == "m"):
        numero = numero * 1
        elif (medidaPasar == "km"):
        numero = numero / 1000
        elif(medidaPasar = "mm"):
        numero = numero * 1000

    Case "km":
        if (medidaPasar == "km"):
        numero = numero * 1
        elif (medidaPasar == "m"):
        numero = numero * 1000
        elif(medidaPasar = "mm"):
        numero = numero * 100000
print(numero)
```
---
**7. Acierta el número**
```
from random import randint

numero = randint(0,100)

while usuario != numero:
    usuario = int(input("Introduce y averiga el numero del 1 al 100"))
    if usuario < numero:
        print("El numero más alto")
    elif intento > numero:
        print("El numero más bajo")
    else:
        print("Felicidades has acertado")
```
---
**8. Piedra, papel, tijeras, lagarto, Spock**
```
from random import choice
puntosJugador = 0
puntosMaquina = 0
puntosEmpate = 0
opciones = ['piedra','papel','tijera','lagarto','Spock']

while puntosJugador < 5 or puntosMaquina < 5 or puntosEmpate < 5:
    jugador = input("Elige entre 'piedra','papel','tijera','lagarto','Spock'")
    ordenador = choice(opciones)
    match(jugador)
        case 'piedra':
            if ordenador == 'papel' or ordenador == 'Spock':
               puntosMaquina += 1
            elif ordenador == 'lagarto' or ordenador == 'tijera':
                puntosJugador += 1
            else:
                puntosEmpate += 1
        case 'papel':
            if ordenador == 'lagarto' or ordenador == 'tijera':
               puntosMaquina += 1
            elif ordenador == 'piedra' or ordenador == 'Spock':
                puntosJugador += 1
            else:
                puntosEmpate += 1
        case 'tijera':
            if ordenador == 'piedra' or ordenador == 'Spock':
               puntosMaquina += 1
            elif ordenador == 'papel' or ordenador == 'lagarto':
                puntosJugador += 1
            else:
                puntosEmpate += 1
        case 'lagarto':
            if ordenador == 'piedra' or ordenador == 'tijera':
               puntosMaquina += 1
            elif ordenador == 'papel' or ordenador == 'Spock':
                puntosJugador += 1
            else:
                puntosEmpate += 1
        case 'Spock':
            if ordenador == 'papel' or ordenador == 'lagarto':
               puntosMaquina += 1
            elif ordenador == 'tijera' or ordenador == 'piedra':
                puntosJugador += 1
            else:
                puntosEmpate += 1
```
---
**9.- Secuencia de Fibonacci**
```
numeroInput = int(input("Introduce un numero"))
a,b = 1,1

for numeros in range(numeroInput):
    print(b)
    a, b = b, a + b
```