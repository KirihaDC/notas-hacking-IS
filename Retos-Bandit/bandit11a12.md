# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** , donde todas las letras minúsculas (az) y mayúsculas (AZ) se han girado 13 posiciones
## Datos de acceso
Usuario: bandit11
Password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
## Solucion
``` shell
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M]
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```

## Notas adicionales

## Referencias