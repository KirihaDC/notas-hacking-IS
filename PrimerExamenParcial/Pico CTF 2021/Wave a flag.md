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
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm      
zsh: permiso denegado: ./warm
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm             
Hello user! Pass me a -h to learn what I can do!
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: 

picoCTF{s4n1ty_v3r1f13d_2aa22101}
```

## Notas
Debes tomar en cuenta los permisos, aveces solo basta con tener los permisos para pasar de nivel y tener acceso a algunas funciones para poder resover el reto y sacar la bandera.

## Referencias
 [linck del programa](https://mercury.picoctf.net/static/fc1d77192c544314efece5dd309092e3/warm)