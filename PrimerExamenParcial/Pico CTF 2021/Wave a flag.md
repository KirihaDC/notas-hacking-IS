# Wave a flag

## Objetivo 
Descripción:
¿Puede invocar banderas de ayuda para una herramienta o binario? [Este programa](https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm) tiene información extraordinariamente útil...

Sugerencias:
Este programa solo funcionará en webshell u otra computadora con Linux.

Para acceder al archivo en su shell, ingrese lo siguiente en el indicador de Terminal:`$ wget https://mercury.picoctf.net/static/cfea736820f329083dab9558c3932ada/warm`

Ejecute este programa ingresando lo siguiente en el indicador de Terminal: `$ ./warm`, pero primero tendrá que hacerlo ejecutable con`$ chmod +x warm`

-h y --help son los argumentos más comunes que se dan a los programas para obtener más información de ellos.

No todos los programas implementan funciones de ayuda como -h y --help.

## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ cd Descargas
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm      
zsh: permiso denegado: ./warm
                                                                         
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ls -la
total 800
drwxr-xr-x  2 kiriha kiriha   4096 sep 26 22:00 .
drwxr-xr-x 16 kiriha kiriha   4096 sep 26 21:39 ..
-rw-r--r--  1 kiriha kiriha  14551 sep 26 13:53 file
-rw-r--r--  1 kiriha kiriha     34 sep 26 21:32 flag
-rw-r--r--  1 kiriha kiriha 776032 sep 26 12:54 strings
-rw-r--r--  1 kiriha kiriha  10936 sep 26 22:00 warm
                                                                         
┌──(kiriha㉿kali)-[~/Descargas]
└─$ chmod 777 warm                                        
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ls -la        
total 800
drwxr-xr-x  2 kiriha kiriha   4096 sep 26 22:00 .
drwxr-xr-x 16 kiriha kiriha   4096 sep 26 21:39 ..
-rw-r--r--  1 kiriha kiriha  14551 sep 26 13:53 file
-rw-r--r--  1 kiriha kiriha     34 sep 26 21:32 flag
-rw-r--r--  1 kiriha kiriha 776032 sep 26 12:54 strings
-rwxrwxrwx  1 kiriha kiriha  10936 sep 26 22:00 warm
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm             
Hello user! Pass me a -h to learn what I can do!
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: 

//Revisar Notas
```

## Notas
Debes tomar en cuenta los permisos, aveces solo basta con tener los permisos para pasar de nivel y tener acceso a algunas funciones para poder resover el reto y sacar la bandera.

Nota del codigo: No pude sacar la bandera por errores que me da la maquina virtual al momento de arrancarlo pero la solucion si es la de arriba, cuando pueda hacer funcionar la maquina virtual actualizare los retos para subir las banderas a mis codigos de obsidian y al picoCTF para que se queden registradas de igual forma en la plataforma y salgan los puntos en mi perfil.

## Referencias
 [linck del programa](https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm)