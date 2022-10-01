# PW Crack 3

## Objetivo 
¿Puedes descifrar la contraseña para obtener la bandera?Descargue el verificador de contraseñas [aquí](https://artifacts.picoctf.net/c/25/level3.py) y también necesitará el [indicador](https://artifacts.picoctf.net/c/25/level3.flag.txt.enc) cifrado y el [hash](https://artifacts.picoctf.net/c/25/level3.hash.bin) en el mismo directorio.Hay 7 contraseñas potenciales con 1 siendo correcta. Puede encontrarlos examinando el script del verificador de contraseñas.

## Solución 
``` shell
┌──(kiriha㉿kali)-[~/Descargas]
└─$ nano level3.py 

┌──(kiriha㉿kali)-[~/Descargas]
└─$ nano level3.py

┌──(kiriha㉿kali)-[~/Descargas]
└─$ python level3.py
Please enter correct password for flag: 1ea2
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_6f98a49f}
```

## Notas
Debes usar el comando bvi en el level3.hash.bin para analizarlo y sacar la contraseña correcta que se encuentra en el level3.py para que la coloques de forma correcta en el ejecutable.

## Referencias
[Descargar contraseña](https://artifacts.picoctf.net/c/25/level3.py)
[Descargar indicador](https://artifacts.picoctf.net/c/25/level3.flag.txt.enc)
[Descargar hash](https://artifacts.picoctf.net/c/25/level3.hash.bin)
