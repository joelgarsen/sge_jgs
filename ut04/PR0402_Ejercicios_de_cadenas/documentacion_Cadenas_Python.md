**1. Contar vocales y consonantes**
```
cadena = input("Introduce una cadena")
vocales = 0
consonantes = 0
for caracteres in cadena:
    if caracteres == 'a' or caracteres == 'e' or caracteres == 'i' or caracteres == 'o' or caracteres == 'u':
        vocales += 1
    else:
        consonantes += 1
print("Vocales")
print(vocales)
print("Consonantes")
print(consonantes)
```
---
**2. Invertir una cadena**
```
cadena = input("Introduce una cadena")
print(cadena[::-1])
```
---
**3. Verificar palíndromo**
```
cadena = input("Inserte una cadena")

cadenaLimpia = cadena.strip(" ").lower()

if (cadenaLimpia == cadenaLimpia[::-1]):
    print("Es palindromo")
else:
    print("No es palindromo")
```
---
**4. Contar palabras**
```
cadena = input("Inserte una cadena")
contador = 0
cadenaLimpia = cadena.split(" ")
for i in cadenaLimpia:
    contador+=1
print("Palabras contadas")
print(contador)

```
---
**5. Eliminar caracteres repetidos**
```
cadena = input("Inserte una cadena")
cadenaLista = []
for caracter in cadena:
    if(not caracter in cadenaLista):
        cadenaLista.extend(caracter)
print(cadenaLista)
```
---
**6. Mayúsculas y minúsculas**
```
cadena = input("Inserte una cadena")

cadenaModificada = cadena.swapcase()

print(cadenaModificada)
```
---
**7. Invertir palabras de una cadena**
```
cadena = input("Inserte una cadena")
cadenaLimpia = cadena.split(" ")
cadenaLimpia.reverse()
print(cadenaLimpia)
```
---
**8. Anagrama**
```
cadenaUno = input("Inserte una cadena")
cadenaDos = input("Inserte una cadena")

listaCadenaUno = [i for i in cadenaUno]
listaCadenaDos = [i for i in cadenaDos]

listaOrdenadaUno = listaCadenaUno.sort()
listaOrdenadaDos = listaCadenaDos.sort()

if(listaOrdenadaUno == listaOrdenadaDos):
    print("Es un anagrama")
else:
    print("No es un anagrama")
```
---
**9. Frecuencia de caracteres**
```
cadena = input("Inserte una cadena")
frecuencia = {}
for caracter in cadena:
    if (caracter in frecuencia):
        frecuencia[caracter] +=1
    else:
        frecuencia[caracter] = 1
print(frecuencia)
```
---
**10. Quitar caracteres alfanuméricos**
```
import re
cadena = input("Inserte una cadena")
cadenaLimpia = re.sub('[^a-zA-Z0-9]', '', cadena)
print(cadenaLimpia)
```
---
**11. Transformar a camelCase**
```
cadena = "Hola mundo"
cadenaLimpia = cadena.lower.split(" ")
caracterLista = cadenaLimpia[0]
for caracter in cadenaLista[1:]: 
  caracterLista += palabra.capitalize()
print(caracterLista)
```
---
**12. Codificación RLE (Run-Length Enconding)**
```
def funcion(cadena):
    resultado = ""
    contador = 1
    for caracter in range(1, len(cadena)):
        if cadena[caracter] == cadena[caracter - 1]:
            contador += 1
        else:
            resultado += cadena[caracter - 1] + str(contador)
    resultado += cadena[-1] + str(contador)
    return resultado
```
---
**13. Decodificar RLE**
```
```
---
**14. Formateo de cadenas con plantillas**
```
```
---
**15. Comparar cadenas por valor ASCII**
```
```
---
**16. Contar la longitud de palabra más larga**
```
```
---
**17. Formatear número con separador de miles**
```
```
---
**18. Rotar caracteres de una cadena**
```
```

