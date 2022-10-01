# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** , que contiene datos codificados en base64
## Datos de acceso
Usuario: bandit10
Password: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
## Solucion
```shell
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt
VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==
bandit10@bandit:~$ cat data.txt | base64
VkdobElIQmhjM04zYjNKa0lHbHpJRWxHZFd0M1MwZHpSbGM0VFU5eE0wbFNSbkZ5ZUVVeGFIaFVU
a1ZpVlZCU0NnPT0K
bandit10@bandit:~$ cat data.txt | base64 -d
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```

## Notas adicionales
El base64 -d sirve para poder 
## Referencias

