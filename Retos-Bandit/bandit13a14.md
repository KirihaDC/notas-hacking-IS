# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en **/etc/bandit_pass/bandit14 y solo puede leerla el usuario bandit14** . Para este nivel, no obtiene la siguiente contraseña, pero obtiene una clave SSH privada que puede usarse para iniciar sesión en el siguiente nivel. **Nota:** **localhost** es un nombre de host que se refiere a la máquina en la que está trabajando
## Datos de acceso
Usuario: bandit13
Password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
## Solucion
```shell
bandit13@bandit:~$ ls
sshkey.private
bandit13@bandit:~$ cat sshkey.private
bandit13@bandit:~$ ssh -i sshkey.private bandit14@localhost
bandit14@bandit:~$ ls
bandit14@bandit:~$ cat
cat        catchsegv  catman
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```

## Notas adicionales

## Referencias

