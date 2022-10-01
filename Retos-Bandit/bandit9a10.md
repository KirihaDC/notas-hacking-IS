# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** en una de las pocas cadenas legibles por humanos, precedida por varios caracteres '='.
## Datos de acceso
Usuario: bandit9
Password: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
## Solucion
```shell
bandit9@bandit:~$ strings data.txt | grep ==
========== the*2i"4
========== password
Z)========== is
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
bandit9@bandit:~$ strings -n 30 data.txt | grep ==
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```

## Notas adicionales
El comando grep filtra todos los archivos por los que tengan una cadena de caracteres especifica y el -n "numero" por una cantidad especifica de los caracteres
## Referencias

