# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** y es la única línea de texto que aparece una sola vez.
## Datos de acceso
Usuario: bandit8
Password: cvX2JJa4CFALtqS87jk27qwqGhBM9plV
## Solucion
bandit8@bandit:~$ ls
data.txt
bandit8@bandit:~$ cat data.txt | sort | uniq -c^C
bandit8@bandit:~$ cat data.txt | sort | uniq -d^C
bandit8@bandit:~$ cat data.txt | sort | uniq -u^C
bandit8@bandit:~$ cat data.txt | sort | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
## Notas adicionales
El sort sive para ordenar todos los archivos 
## Referencias

https://ryanstutorials.net/linuxtutorial/piping.php