# Bandit

## Objetivo
La contraseña para el siguiente nivel se puede recuperar enviando la contraseña del nivel actual al **puerto 30000 en localhost** .
## Datos de acceso
Usuario: bandit14
Password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
## Solucion
```shell
bandit14@bandit:~$ ls
bandit14@bandit:~$ nc localhost 30000
^C
bandit14@bandit:~$ nc -v localhost 30000
localhost [127.0.0.1] 30000 (?) open
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr
```

## Notas adicionales

## Referencias

