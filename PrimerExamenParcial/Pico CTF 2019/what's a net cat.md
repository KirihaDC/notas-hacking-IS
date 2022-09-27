# what's a net cat

## Objetivo 
Descripción:
Usar netcat (nc) va a ser muy importante. ¿Puede conectarse a  `jupiter.challenges.picoctf.org` en el puerto `41120` para obtener la bandera?

Sugerencias:
nc [tutorial](https://linux.die.net/man/1/nc)


## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ nc jupiter.challenges.picoctf.org 41120
You're on your way to becoming the net cat master
picoCTF{nEtCat_Mast3ry_3214be47}
```

## Notas
Para entrar recuerda que debes de poner el servidor y el puerto, similar a los retos bandit:
nc jupiter.challenges.picoctf.org 41120

## Referencias
[nc](https://linux.die.net/man/1/nc)