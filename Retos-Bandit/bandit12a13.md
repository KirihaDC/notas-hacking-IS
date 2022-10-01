# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** , que es un volcado hexadecimal de un archivo que ha sido comprimido repetidamente. Para este nivel, puede ser útil crear un directorio bajo /tmp en el que pueda trabajar usando mkdir. Por ejemplo: mkdir /tmp/myname123. Luego copie el archivo de datos usando cp, y cámbiele el nombre usando mv (¡lea las páginas de manual!)
## Datos de acceso
Usuario: bandit12
Password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
## Solucion
```shell
bandit12@bandit:~$ ls
data.txt
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```

## Notas adicionales
Descomprimir arcchivos en linux
## Referencias

