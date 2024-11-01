# ProyectoEjemploGit

## Descripción
En el proyecto, creé un programa en Java que muestra un mensaje en la consola (HolaMundo.java) que imprime un mensaje en la consola, inicialmente mostraba "Hola Mundo" en consola, pero después lo modifiqué para que mostrara "Hola Git". Este cambio fue para manejar diferentes commits y versiones en Git.

El objetivo de esta tarea es repasar los comandos básicos de Git, crear un repositorio en GitHub y aprender a utilizar un archivo `.gitignore` para gestionar los archivos que no se deben subir al repositorio y subirlo a GitHub.Aprender a manejar archivos .gitignore y documentos con Markdown.


## Cómo ejecutar el programa
1. Abrir tu terminal
2. ir a la carpeta del proyecto que usaste cd ProyectoEjemploGit
3. Compilar el programa: HolaMundo.java
4. Ejecútarlo: java HolaMundo

## Comandos Git que usé
Utilicé los siguientes comandos:
- `git init` → Para crear mi repositorio en la carpeta ProyectoEjemploGit
- `git add HolaMundo.java` → Para agregar mi programa al primer commit
- `git commit -m "Se agregó el programa de Hola Mundo en Java"` → Mi primer commit
- `git add .gitignore` → Para agregar el archivo que ignora los .log
- `git commit -m "Se agregó el archivo .gitignore"` → Mi segundo commit
- `git add HolaMundo.java` → Para agregar los cambios del mensaje
- `git commit -m "Se actualizó el mensaje en HolaMundo.java"` → Mi tercer commit
- `git remote add origin [URL-del-repositorio]` → Para conectar con GitHub
- `git push -u origin main` → Para subir todo a GitHub

##  Notas sobre el archivo .gitignore:
### ¿Por qué lo creé?
Creé el archivo .gitignore porque necesitaba evitar que algunos archivos se subieran al repositorio. En este  proyecto, quería ignorar específicamente los archivos de registro (.log) que no son necesarios en el control de versiones.
### ¿Qué archivos se ignoran?
- Todos los archivos que terminen en .log (como debug.log)
- Los archivos compilados de Java (.class)

### Para comprobar que debug.log no se subió:
1. Ejecuté `git status` en la terminal
2. Vi que debug.log no aparecía en la lista de archivos sin seguimiento
3. También revisé en GitHub y confirmé que el archivo no estaba ahí

# Muestra
Al ejecutar el programa mostrara "Hola Git" en la consola, y si se busca debug.log en el repositorio de GitHub, no se encontrara porque está siendo ignorado por el Git.