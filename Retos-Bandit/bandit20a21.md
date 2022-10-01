# Bandit

## Objetivo
Hay un binario setuid en el directorio de inicio que hace lo siguiente: establece una conexión con localhost en el puerto que especifique como argumento de la línea de comandos. Luego lee una línea de texto de la conexión y la compara con la contraseña del nivel anterior (bandit20). Si la contraseña es correcta, transmitirá la contraseña para el siguiente nivel (bandit21).

**NOTA:** intente conectarse a su propio demonio de red para ver si funciona como cree
## Datos de acceso
Usuario: bandit20
Password: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
## Solucion
```shell
bandit20@bandit:~$ nc -lnvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &
[1] 365506
bandit20@bandit:~$ Listening on 0.0.0.0 3030

bandit20@bandit:~$ jobs
[1]+  Running                 nc -lnvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &
bandit20@bandit:~$ ./suconnect 3030
Connection received on 127.0.0.1 41100
Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
Password matches, sending next password
NvEJF7oVjkddltPSrdKEFOllh9V1IBcq
[1]+  Done                    nc -lnvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT

NvEJF7oVjkddltPSrdKEFOllh9V1IBcq
```
## Notas adicionales

## Referencias

