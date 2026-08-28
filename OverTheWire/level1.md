Para conseguir la clave para el nivel 2 debemos ingresar al servidor con el usuario bandit1 con el siguiente comando:

**ssh -p 2220 bandit1@bandit.labs.overthewire.org**

Nos pedira la contraseña que encontramos en el nivel anterior la cual era **6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR**

Una vez dentro podemos revisar los archivos que tenemos en el directorio con **ls** y encontraremos un archivo llamado **-**

los archivos nombrados con **-** en el principio normalmente dan problemas por lo cual no podremos utilizar **cat -**

Para revisar el texto del archivo debemos utilizar **cat ./-**

Este comando nos entregara la contraseña del nivel 2 la cual es: **PK8fYLZg2hnHSz83plBL1iEPKdD3QToB**

Cerramos la conexion con **exit**
