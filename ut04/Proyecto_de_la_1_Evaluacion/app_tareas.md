
```python
import datetime
listaTareas = {}

# Funciones
def añadir_Tareas():
    parametroUno = input("Introduce un nombre a la tarea")
    if nombre in listaTareas:
        print("El nombre de esta tarea ya existe")
        return
    parametroDos = int(input("Introduce una prioridad a la tarea"))
    parametroTres = input("Introduce una fecha limite a la tarea")

    listaTareas[parametroUno] = {
        "prioridad": parametroDos,
        "fecha_limite": parametroTres,
        "completada": False
    }

def eliminar_Tareas():
    parametroBorrar = input("Introduce el nombre de la tarea que deseas borrar")
    if parametroBorrar in listaTareas:
        del listaTareas[parametroBorrar]
        print("Tarea eliminada")
    else: 
        print("La tarea no existe")
    
def listar_Tareas():
    if not listaTareas:
        print("No hay tareas")
        return
    for nombre in listaTareas.items():
        estado = "completada" if detalles["completada"] else "Pendiente"
        print(f"Tarea: {nombre}, Prioridad: {listaTareas['prioridad']}, Fecha Limite: {listaTareas['fecha_limite']}, Estado: {estado}")
        
def marcarCompletada_Tareas():
    parametroUno = ("Introduce el nombre de la tarea que deseas")
    if parametroUno in listaTareas:
        listaTareas[nombre]["completada"] = True
        print("Tarea marcada")
    else:
        print("Tarea no completada")

def vencidas_Tareas():
    hoy = datetime.date.today()
    vencidas = False
    print("Tareas vencidas")
    for nombre in listaTareas.items():
        if {listaTareas['fecha_limite']} < hoy and not detalles{listaTareas['completada']}:
            print(f"Tarea: {nombre}, Prioridad: {listaTareas['prioridad']}, Fecha Limite: {listaTareas['fecha_limite']}")
            vencidas = True
        else:
            print("No hay tareas vencidas")

#Menu
while True:
    print("Gestor de tareas")
    print("---------------------------------")
    print("1. Añadir tarea")
    print("2. Eliminar tarea")
    print("3. Listar tareas")
    print("4. Marcar tarea como completada")
    print("5. Tareas vencidas")
    print("6. Salir y guardar")
    print("---------------------------------")
    eleccion = input("Seleccione un numero: ")

    if eleccion == "1":
        añadir_Tareas()
    elif eleccion == "2":
        eliminar_Tareas()
    elif eleccion == "3":
        listar_Tareas()
    elif eleccion == "4":
        marcarCompletada_Tareas()
    elif eleccion == "5":
        vencidas_Tareas()
    elif eleccion == "6":
        print("Saliendo...")
        break
    else:
        print("Opcion no valida")
```