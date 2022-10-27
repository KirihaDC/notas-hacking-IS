# WhitePages

## Objetivo
Dejé de usar YellowPages y pasé a WhitePages... ¡pero [la página que me dieron](https://jupiter.challenges.picoctf.org/static/95be9526e162185c741259a75dffa0ab/whitepages.txt) está en blanco!

## Solucion
Para resolver este reto debemos usar el HEX EDITOR para ver lo que contiene el archivo, al abrirlo podemos ver que tenemos el espacio estándar ( `0x20`) y el Unicode EM SPACE ( `0xE2 0x80 0x83`):

``` shell
┌──(kiriha㉿kali)-[~/Descargas]
└─$ xxd whitepages.txt | head
00000000: e280 83e2 8083 e280 83e2 8083 20e2 8083  ............ ...
00000010: 20e2 8083 e280 83e2 8083 e280 83e2 8083   ...............
00000020: 20e2 8083 e280 8320 e280 83e2 8083 e280   ...... ........
00000030: 83e2 8083 20e2 8083 e280 8320 e280 8320  .... ...... ... 
00000040: 2020 e280 83e2 8083 e280 83e2 8083 e280    ..............
00000050: 8320 20e2 8083 20e2 8083 e280 8320 e280  .  ... ...... ..
00000060: 8320 20e2 8083 e280 83e2 8083 2020 e280  .  .........  ..
00000070: 8320 20e2 8083 2020 2020 e280 8320 e280  .  ...    ... ..
00000080: 83e2 8083 e280 83e2 8083 2020 e280 8320  ..........  ... 
00000090: e280 8320 e280 8320 e280 83e2 8083 e280  ... ... ........
``` 

Con esto anterior mencionado solo debemos crear un archivo python con el que podamos decifrar el contenio, el cual al ser ejecutado nos terminara arrojando la bandera que vendria siendo la siguiente:
picoCTF{not_all_spaces_are_created_equal_7100860b0fa779a5bd8ce29f24f586dc}

## Notas adicionales

## Referencias