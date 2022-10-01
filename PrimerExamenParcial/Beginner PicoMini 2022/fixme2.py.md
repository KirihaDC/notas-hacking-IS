# fixme2.py

## Objetivo 
Solucione el error de sintaxis en el script de Python para imprimir la bandera.

## Solución 
``` shell
┌──(kiriha㉿kali)-[~/Descargas]
└─$ python fixme2.py
  File "/home/kiriha/Descargas/fixme2.py", line 22
    if flag = (""):
       ^^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
                                                                                                                                                                       
┌──(kiriha㉿kali)-[~/Descargas]
└─$ nano fixme2.py  
                                                                                                                                                                       
┌──(kiriha㉿kali)-[~/Descargas]
└─$ python fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
```

## Notas
Recuerda que debes usar el comando nano para verificar que este todo correcto en el codigo para que se pueda ejecutar en python.

## Referencias
[Descargar secuencia de comando de python](https://artifacts.picoctf.net/c/66/fixme2.py)
