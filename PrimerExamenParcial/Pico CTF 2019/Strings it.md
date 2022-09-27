# Strings it

## Objetivo 
Descripción:
¿Puedes encontrar el indicador en el  [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) sin ejecutarlo?

Sugerencias:
[strings](https://linux.die.net/man/1/strings)


## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ ls
Descargas   Escritorio  Música      Público
Documentos  Imágenes    Plantillas  Vídeos
                                                                             
┌──(kiriha㉿kali)-[~]
└─$ cd Descargas 
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ls
strings
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ strings strings | grep picoCTF
//Revisar notas

```

## Notas
Para poder sacar las banderas e inspeccionar el archivo debes estar posicionado en la carpeta correspondiente

Nota del codigo: No pude sacar la bandera por errores que me da la maquina virtual al momento de arrancarlo pero la solucion si es la de arriba, cuando pueda hacer funcionar la maquina virtual actualizare los retos para subir las banderas a mis codigos de obsidian y al picoCTF para que se queden registradas de igual forma en la plataforma y salgan los puntos en mi perfil.

## Referencias
[strings](https://linux.die.net/man/1/strings)