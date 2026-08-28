Para solucionar el nivel 3 primero debemos conectarnos por medio de ssh a ssh -p 2220 bandit3@bandit.labs.overthewire.org con el usuario bandit3

Revisamos los archivos de la carpeta y nos encontramos con otra carpeta dentro de nuestro directorio local la cual se llama **inhere**

Ingresamos a la carpeta con el comando **cd inhere**

Revisamos nuevamente los archivos con **ls** y no nos mostrara nada debido a que el archivo está oculto

Utilizamos el comando **find** y nos mostrará que existe un archivo llamado **...Hiding-From-You** Tambien podemos realizar **ls -la** y nos mostrara todos los archivo incuyendo los ocultos

Ejecutamos **cat ...Hiding-From-You** para leer el contenido y obtener la contraseña del nivel 4 la cual es: **xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq**

Cerramos la sesión con **exit**
