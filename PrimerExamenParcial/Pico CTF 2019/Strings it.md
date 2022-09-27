# Strings it

## Objetivo 
Descripción:
¿Puedes encontrar el indicador en el  [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) sin ejecutarlo?

Sugerencias:
[strings](https://linux.die.net/man/1/strings)


## Solución 
``` shell           
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ls
strings
                                
┌──(kiriha㉿kali)-[~/Descargas]
└─$ strings strings | grep picoCTF
picoCTF{5tRIng5_1T_7f766a23}

```

## Notas
Para poder sacar las banderas e inspeccionar el archivo debes estar posicionado en la carpeta correspondiente


## Referencias
[strings](https://linux.die.net/man/1/strings)