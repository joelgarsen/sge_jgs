**Buscar valor en un diccionario**
```
productos = {
    "Manzana": [4],
    "Pera": [5],
    "Platano": [7],
}

cadena = input("Ingrese nombre de una fruta")

if cadena in productos:
    print(productos[cadena])
else:
    print("No está disponible")
```
---
**Contar elementos en un diccionario**
```
productos = {
    "Electrónica": ["Smartphone", "Laptop", "Tablet", "Auriculares", "Smartwatch"],
    "Hogar": ["Aspiradora", "Microondas", "Lámpara", "Sofá", "Cafetera"],
    "Ropa": ["Camisa", "Pantalones", "Chaqueta", "Zapatos", "Bufanda"],
    "Deportes": ["Pelota de fútbol", "Raqueta de tenis", "Bicicleta", "Pesas", "Cuerda de saltar"],
    "Juguetes": ["Muñeca", "Bloques de construcción", "Peluche", "Rompecabezas", "Coche de juguete"],
}
numeroDeCategorias: len(productos)
print("Numero de categorias" + str(numeroDeCategorias))

for categoria, producto in productos.items():
    print("Categoria: " + str(categoria) + " | Numero de productos: " + str(producto))

for products in productos.values():
    print("Total de productos: " + str(products))
```
---
**Contador de frecuencias de palabras**
```
cadena = input("Pon una frase")
cadenaMinisculas = cadena.lower()
cadenaSeparada = cadena.split()
frecuencia = {}

for palabra in cadenaSeparada:
    if palabra in frecuencia:
        frecuencia[palabra] += 1
    else:
        frecuencia[palabra] = 1

print("Frecuencia:")
for palabra, item in frecuencia.items():
    print(str(palabra) + " : " + str(item))
```
---
**Diccionario de listas**
```
asignaturas = {
    "Matemáticas": ["Ana", "Carlos", "Luis", "María", "Jorge"],
    "Física": ["Elena", "Luis", "Juan", "Sofía"],
    "Programación": ["Ana", "Carlos", "Sofía", "Jorge", "Pedro"],
    "Historia": ["María", "Juan", "Elena", "Ana"],
    "Inglés": ["Carlos", "Sofía", "Jorge", "María"],
}

while True:
    print("Elige una opcion")
    print("---------------------------------")
    print("1. Añadir estudiante")
    print("2. Eliminar estudiante")
    print("3. Listar estudiantes")
    print("4. Salir")
    print("---------------------------------")
    eleccion = input("Seleccione un numero: ")

    if eleccion == "1":
        asignatura = input("Ingrese el nombre de la asignatura")
        estudiante = input("Ingrese el nombre del estudiante")
        def_Añadir(asignatura, estudiante)
    elif eleccion == "2":
        asignatura = input("Ingrese el nombre de la asignatura")
        estudiante = input("Ingrese el nombre del estudiante")
        def_Quitar(asignatura)
    elif eleccion == "3":
        asignatura = input("Ingrese el nombre de la asignatura")
        def_Listar(asignatura)
    elif eleccion == "4":
        print("Saliendo...")
        break
    else:
        print("Opcion no valida")

def_Añadir(asignatura, estudiante):
    if asignatura in asignaturas:
        if estudiante not in asignaturas[asignatura]:
            asignaturas[asignatura].append(estudiante)
            print(str(estudiante) + " matriculado en " + str(asignatura))
        else:
            print("El alumno ya esta matriculado")
    else:
        print("La asignatura no existe")
-
def_Quitar(asignatura, estudiante):
    if asignatura in asignaturas:
        if estudiante not in asignaturas[asignatura]:
            asignaturas[asignatura].remove(estudiante)
            print(str(estudiante) + " eliminado de " + str(asignatura))
        else:
            print("El alumno no esta matriculado")
    else:
        print("La asignatura no existe")
-
def_Listar(asignatura):
    if asignatura in asignaturas:
        print("Asignaturas: " + str(asignatura) + ": " + ", ".join(asignaturas[asignatura]))
    else:
        print("La asignatura no existe")
```
---
**Diccionario invertido**
```
productos = {
    "Manzana": [4],
    "Pera": [5],
    "Platano": [7],
}

productosInvertido = intercambio(productos)

print(productosInvertido)


def intercambio(productos):
    intercambio = {valor: clave for clave, valor in productos.items()}
    return intercambio
```
---
**Combinar dos diccionarios**
```
productosUno = {
    "Manzana": [4],
    "Pera": [5],
    "Platano": [7],
}

productosDos = {
    "Kiwi": [6],
    "Naranja": [3],
    "Granada": [4],
}

productosCombinados = {}

for producto, precio in productosUno.items():
    productosCombinados[producto] = precio

for producto, precio in productosUno.items():
    if producto in productosCombinados:
        productosCombinados[producto] += precio
    else:
        productosCombinados[producto] = precio

print("Productos combinados")
for producto, precio in productosCombinados.items():
    print(str(producto) + " : " + str(precio))
```
---