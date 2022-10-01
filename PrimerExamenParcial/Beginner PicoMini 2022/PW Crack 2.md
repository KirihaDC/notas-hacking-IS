# PW Crack 2

## Objetivo 
¿Puedes descifrar la contraseña para obtener la bandera?Descargue el verificador de contraseñas [aquí](https://artifacts.picoctf.net/c/16/level2.py) y también necesitará el [indicador](https://artifacts.picoctf.net/c/16/level2.flag.txt.enc) cifrado en el mismo directorio.

## Solución 
``` shell
┌──(kiriha㉿kali)-[~/Descargas]
└─$ nano level2.py          
                                                                                                                                                                      
┌──(kiriha㉿kali)-[~/Descargas]
└─$ python          
Python 3.10.5 (main, Jun  8 2022, 09:26:22) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36))
de76
>>> 
                                                                                                                                                                      
┌──(kiriha㉿kali)-[~/Descargas]
└─$ python level2.py  
Please enter correct password for flag: de76
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}
```

## Notas
Verificar que el codigo este correcto en el archivo con el comando nano para que no marque errores a la hora de ejecutar.

## Referencias
[Descargar contraseña](https://artifacts.picoctf.net/c/16/level2.py)
[Descargar indicador](https://artifacts.picoctf.net/c/16/level2.flag.txt.enc)
