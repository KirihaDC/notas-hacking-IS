# Glitch Cat

## Objetivo 
¡Nuestro servicio de impresión de banderas ha comenzado a fallar!`$ nc saturn.picoctf.net 65353`

## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ nc saturn.picoctf.net 65353
'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'
                                                                                                                                                                      
┌──(kiriha㉿kali)-[~]
└─$ python          
Python 3.10.5 (main, Jun  8 2022, 09:26:22) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print('picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}')
picoCTF{gl17ch_m3_n07_9c42a45d}
```

## Notas
Recuerda que debes usar Python para sacar la parte que falta de la bandera usando el codido print() para impirmir la bandera completa.

## Referencias