# **PR0603**

## Paso 1 (Añadir creacion de directorio y archivos)
Dentro de donde tenemos todos los repositorio de **"Docker"** vamos a la carpeta **addons** para abrir una terminal dentro de esta.
(Teniendo el Docker encendido) Abrimos una terminal con el `docker compose exec odoo bash` y acto seguido escribimos el comando `odoo scaffold <NombreQueQuieras> /mnt/extra-addons/`

![Imagen](Captura1.png)

## Paso 2 (Modelo y manifest)

Creamos el modelo junto con todas las restricciones de los campos
![Imagen](2.png)

## Paso 3 (Views)
Escribimos los campos en el views
![Imagen](4.png)

## Paso 4 (Security)
Indicamos los parametros para que reconozca al modulo
![Imagen](3.png)