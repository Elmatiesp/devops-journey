Para solucionar el nivel 2 primero debemos conectarnos por medio de ssh a **ssh -p 2220 bandit2@bandit.labs.overthewire.org** con el usuario bandit2

Revisamos los archivos de la carpeta y nos encontramos con un archivo que empieza con **-** y ademas tiene espacios

Para poder leer este archivo debemos realizar lo que hicimos en el ejercicio anterior pero tambien sumar el uso de comillas "" debido a que el nombre tiene espacios

El comando quedaria de la siguiente manera: **cat ./"--spaces in this filename--"**

Este comando leera el archivo y nos entregara la contraseña para el nivel 3 la cual sería: **7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME**
