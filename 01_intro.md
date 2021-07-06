# Resumen Intro MongoDB

## Instalación de MongoDB Community Server en local para DEV

Descargar paquete msi desde https://www.mongodb.com/try/download/community

Lanzar el asistente (opcional desmarcar la opción de servicio)

## Variable de entorno con ruta

Tanto el servidor (mongod) como la herramienta de línea de comandos o shell (mongo) como
el resto de herramientas se ubican en:

<Unidad>:\Program Files\MongoDB\Server\<versión>\bin

Para lanzar tanto el servidor como la shell desde cualquier ubicación, introducir esa ruta
en las variables de entorno

## Directorio para escrituras en disco

Previo a levantar el servidor necesitamos un directorio para almacenar en disco los archivos
generados por MongoDB

- Directorio por defecto crear <Unidad>:\data\db
- Otro directorio anotar su ruta y usarla con el parametro --dbpath al levantar el servidor

## Levantado servidor

Levantado del servidor del sistema gestor de base de datos

mongod --dbpath <ruta directorio escritura disco> --port <puerto>
si no se especifican usará /data/db como directorio y el puerto 27017

## Conexión con shell o Mongo Compass

Una vez levantado el servidor como trabajamos en MongoDB:

- Herramienta de linea de comandos Shell de mongo
- Herramienta de interfaz gráfica Compass (hay mas)

La shell se ejecuta con mongo <opciones>
