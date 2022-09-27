# First Grep

## Objetivo 
Descripción:
¿Puedes encontrar la bandera en el  [file](https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file)? Esto sería muy tedioso de revisar manualmente, algo me dice que hay una mejor manera.

Sugerencias:
grep [tutorial](https://ryanstutorials.net/linuxtutorial/grep.php)

## Solución 
//Descargamos el file y nos vamos a descargas
``` shell
┌──(kiriha㉿kali)-[~]
└─$ cd Descargas 
                                                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ grep 'picoCTF' file
picoCTF{grep_is_good_to_find_things_5af9d829}
                                                                             
```

## Notas
Usamos grep para viscar picoCTF en file y poder leer la bandera 


## Referencias
grep [tutorial](https://ryanstutorials.net/linuxtutorial/grep.php)