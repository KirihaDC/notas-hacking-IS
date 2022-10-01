# Bandit

## Objetivo
La contraseña para el siguiente nivel se almacena en el archivo **data.txt** junto a la palabra **millionth**
## Datos de acceso
Usuario: bandit7
Password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
## Solucion
```shell
bandit7@bandit:~$ ls
data.txt
bandit7@bandit:~$ grep millionth data.txt
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
bandit7@bandit:~$ cat data.txt | grep millionth
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```

## Notas adicionales
El comando grep sirve para buscar un archivo con una cadena de caracteres especifica
## Referencias
