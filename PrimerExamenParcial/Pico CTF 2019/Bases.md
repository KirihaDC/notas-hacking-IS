# Bases

## Objetivo 
Descripción:
¿Qué significa esto  `bDNhcm5fdGgzX3IwcDM1`? Creo que tiene algo que ver con las bases.


Sugerencias:
Envíe su respuesta en nuestro formato de bandera. Por ejemplo, si su respuesta fue "hola", enviaría "picoCTF{hola}" como bandera.

## Solución 
//detectamos que es una base64
``` shell
┌──(kiriha㉿kali)-[~]
└─$ echo "bDNhcm5fdGgzX3IwcDM1" | base64 -d
l3arn_th3_r0p35

//Revisar notas
```

## Notas
Base64 es un sistema de numeración posicional que usa 64 como base. Es la mayor potencia que puede ser representada usando únicamente los caracteres imprimibles de [ASCII](https://es.wikipedia.org/wiki/ASCII "ASCII"). Esto ha propiciado su uso para codificación de [correos electrónicos](https://es.wikipedia.org/wiki/Correo_electr%C3%B3nico "Correo electrónico"), [PGP](https://es.wikipedia.org/wiki/PGP "PGP") y otras aplicaciones. Todas las variantes famosas que se conocen con el nombre de Base64 usan el rango de caracteres A-Z, a-z y 0-9 en este orden para los primeros 62 dígitos, pero los símbolos escogidos para los últimos dos dígitos varían considerablemente de unas a otras. Otros métodos de codificación como [UUEncode](https://es.wikipedia.org/wiki/UUEncode "UUEncode") y las últimas versiones de [binhex](https://es.wikipedia.org/wiki/Binhex "Binhex") usan un conjunto diferente de 64 caracteres para representar 6 dígitos binarios, pero estos nunca son llamados Base64.

Nota del codigo: No pude sacar la bandera por errores que me da la maquina virtual al momento de arrancarlo pero la solucion si es la de arriba, cuando pueda hacer funcionar la maquina virtual actualizare los retos para subir las banderas a mis codigos de obsidian y al picoCTF para que se queden registradas de igual forma en la plataforma y salgan los puntos en mi perfil.

## Referencias
[strings](https://linux.die.net/man/1/strings)
[base64](https://es.wikipedia.org/wiki/Base64)