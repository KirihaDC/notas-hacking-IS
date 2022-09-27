# Based

## Objetivo 
Descripción:
Para obtener realmente 1337, debe comprender diferentes codificaciones de datos, como hexadecimal o binario. ¿Puedes obtener la bandera de este programa para demostrar que estás en camino de convertirte en 1337? Conectar con `nc jupiter.challenges.picoctf.org 29956`.

Sugerencias:
Escuché que Python puede convertir cosas.
Puede ser útil tener varias ventanas abiertas.

## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ nc jupiter.challenges.picoctf.org 29956
Let us see how data is stored
computer
Please give the 01100011 01101111 01101101 01110000 01110101 01110100 01100101 01110010 as a word.
...
you have 45 seconds.....

Input:
computer
Please give me the  143 157 155 160 165 164 145 162 as a word.
Input:
computer
Please give me the 6f76656e as a word.
Input:
oven
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_b375bb16}
```

## Notas
Para entrar recuerda que debes de poner el servidor y el puerto, similar a los retos bandit:
nc jupiter.challenges.picoctf.org 25103
Tambien podemos usar herramientas externas para resolver los retos, como para convertir los hexadecimales y los octal

## Referencias
[nc](https://linux.die.net/man/1/nc)
[convertidor de binario y hexadecimal](https://www.rapidtables.com/convert/number/binary-to-ascii.html)
[convertidor de octal](http://www.unit-conversion.info/texttools/octal/)