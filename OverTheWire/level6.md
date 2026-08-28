Para solucionar el nivel 6 primero debemos conectarnos por medio de ssh a ssh -p 2220 bandit6@bandit.labs.overthewire.org con el usuario bandit6

Revisamos las carpetas con el comando **ls** y no encontraremos nada debido a que nos dice que en alguna parte del servidor se encuentra el archivo

Para ir a la carpeta root utilizamos **cd ..** 2 veces ahi podremos buscar el archivo con las siguientes caracteristicas:

owned by user bandit7  
owned by group bandit6  
33 bytes in size

Utilizamos el comando **find -type f -user bandit7 -group bandit6 -size 33c** esto nos entregara una lista de mensajes con permission denied para eliminar estos mensajes de error utilizamos:

**find -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null** lo cual redirige todos los mensajes de error a un "agujero negro" descarta todos esos mensajes y solo deja los validos

Nos mostrara el siguiente mensaje: **/var/lib/dpkg/info/bandit7.password**

Tambien podemos realizar la busqueda sin hacer los **cd ..** solo agregando / despues de find 

**find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null**

Para ver la contraseña dentro del archivo utilizamos: **cat ./var/lib/dpkg/info/bandit7.password** y nos entrega la contraseña del nivel 7 la cual es **Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3**

cerramos la sesion con **exit**
