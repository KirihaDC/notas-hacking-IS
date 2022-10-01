# Bandit

## Objetivo
La contraseña para el siguiente nivel se puede recuperar enviando la contraseña del nivel actual al **puerto 30001 en localhost** usando encriptación SSL.

**Nota útil: ¿Obtienes "HEARTBEATING" y "Read R BLOCK"? Use -ign_eof y lea la sección "COMANDOS CONECTADOS" en la página de manual. Junto a 'R' y 'Q', el comando 'B' también funciona en esta versión de ese comando...**
## Datos de acceso
Usuario: bandit15
Password: jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
## Solucion
```shell
bandit15@bandit:~$ openssl s_client -connect localhost:30001
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
Correct!
JQttfApK4SeyHwDlI9SXGR50qclOAil1
```

## Notas adicionales

## Referencias

