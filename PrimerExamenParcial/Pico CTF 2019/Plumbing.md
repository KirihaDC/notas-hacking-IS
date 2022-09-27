# Plumbing

## Objetivo 
A veces necesita manejar datos de proceso fuera de un archivo. ¿Puedes encontrar una manera de mantener la salida de este programa y buscar la bandera? Conectar a `jupiter.challenges.picoctf.org 4427.

Sugerencias:
Recuerda que el formato de la bandera es picoCTF{XXXX}
¿Qué es una pipa? No, no ese tipo de pipa... Este [tipo](http://www.linfo.org/pipes.html)

## Solución 
``` shell
//Es posible combinar dos comandos para que nos de directamente la bandera solo agregamos el grep picoCTF.
┌──(kiriha㉿kali)-[~]
└─$ nc jupiter.challenges.picoctf.org 4427 | grep picoCTF

//Revisar notas
```

## Notas
Recuerda que podemos agregar el grep para facilitar la busqueda de la bandera y debemos usar el tipo de cliente-servidor como con los restos bandit para acceder a nuestra bandera.

Nota del codigo: No pude sacar la bandera por errores que me da la maquina virtual al momento de arrancarlo pero la solucion si es la de arriba, cuando pueda hacer funcionar la maquina virtual actualizare los retos para subir las banderas a mis codigos de obsidian y al picoCTF para que se queden registradas de igual forma en la plataforma y salgan los puntos en mi perfil.



## Referencias
[nc](https://linux.die.net/man/1/nc)
[convertidor de binario y hexadecimal](https://www.rapidtables.com/convert/number/binary-to-ascii.html)
[convertidor de octal](http://www.unit-conversion.info/texttools/octal/)