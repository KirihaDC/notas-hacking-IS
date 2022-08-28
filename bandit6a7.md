# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena **en algún lugar del servidor** y tiene todas las siguientes propiedades:

-   propiedad del usuario bandit7
-   propiedad del grupo bandit6
-   33 bytes de tamaño
## Datos de acceso
Usuario: bandit6
Password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7
## Solucion
bandit6@bandit:~$ ls
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
## Notas adicionales
El comando file sirve para buscar en toda la raiz y el ulitmo codigo despues del sirze sirve para poder ocultar todos los archivos que tengan denegado el acceso
## Referencias

