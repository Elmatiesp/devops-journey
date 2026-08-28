Para solucionar el nivel 5 primero debemos conectarnos por medio de ssh a ssh -p 2220 bandit5@bandit.labs.overthewire.org con el usuario bandit5

Revisamos las carpetas con el comando **ls**

Encontramos una carpeta llamada inhere ingresamos con el comando **cd inhere**

Revisamos los archivos que contiene la carpeta inhere y encontramos muchas carpetas con archivos 

y si utilizamos el comand **find ./*** nos muestra muchos archivos pero el ejercicio nos dice que la contraseña esta dentro de un archivo con las siguientes caracteristicas:

human-readable  
1033 bytes in size  
not executable

Para encontrar ese archivo podemos utilizar el comando **find -type f -readable -size 1033c** este comando busca archivos de tipo archivo que sean de lectura para humanos y de un tamaño de 1033 bytes

El comando nos entrega que solamente hay un archivo con esas caracteristicas el cual es **./maybehere07/.file2**

Podemos realizar el comando **cat ./maybehere07/.file2** para leer el archivo que se encuentra en la carpeta maybehere07 llamado .file2

Y nos dice que la contraseña para el nivel 6 es la siguiente: **pXa26xhMWaC2SvDotA4r9EgZkulOeSBW**

cerramos la sesion con **exit**
