# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en un archivo oculto en el directorio **inhere** .
## Datos de acceso
Usuario: bandit3
Password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
## Solucion
``` shell
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -a
.  ..  .hidden
bandit3@bandit:~/inhere$ cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```

## Notas adicionales
El ls -a sirve para ver archivos que no estan visibles
## Referencias
