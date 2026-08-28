Para solucionar el nivel 4 primero debemos conectarnos por medio de ssh a ssh -p 2220 bandit4@bandit.labs.overthewire.org con el usuario bandit4

Revisamos las carpetas con el comando **ls**

Encontramos una carpeta llamada **inhere** ingresamos con el comando **cd inhere**

Revisamos los archivos que contiene la carpeta **inhere** y encontramos 10 archivos pero el ejercicio nos dice que la contraseña esta en una archivo de lectura para humanos

Para encontrar el archivo que es con lectura para humano utilizamos **file ./*** esto nos entregara la siguiente informacion:

./-file00: data  
./-file01: data  
./-file02: data  
./-file03: data  
./-file04: data  
./-file05: data  
./-file06: OpenPGP Public Key  
./-file07: ASCII text  
./-file08: data  
./-file09: Motorola S-Record; binary data in text format

El archivo de lectura para humanos es el **-file07** de tipo ASCII para leerlo utilizamos el comando **cat ./-file07** y nos entregara la contraseña para el nivel 5 la cual es **6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG**

cerramos la sesion con el comando **exit**
