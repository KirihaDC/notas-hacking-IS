# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en un archivo en algún lugar del directorio **inhere** y tiene todas las siguientes propiedades:

-   legible por humanos
-   1033 bytes de tamaño
-   no ejecutable
## Datos de acceso
Usuario: bandit5
Password: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
## Solucion
```shell
bandit5@bandit:~$ ls
inhere
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ ls
maybehere00  maybehere03  maybehere06  maybehere09  maybehere12  maybehere15  maybehere18
maybehere01  maybehere04  maybehere07  maybehere10  maybehere13  maybehere16  maybehere19
maybehere02  maybehere05  maybehere08  maybehere11  maybehere14  maybehere17
bandit5@bandit:~/inhere$ find . -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```

## Notas adicionales
El comando find . -type f -size 1033c sirve para poder saber el tamaño exacto del archivo
## Referencias
