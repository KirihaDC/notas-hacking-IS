# What Lies Within

## Objetivo
Hay algo en el [edificio](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png) . ¿Puedes recuperar la bandera?

## Solucion
``` shell
┌──(kiriha㉿kali)-[~/Escritorio/PicosCTF/Forence]
└─$ zsteg buildings.png | grep picoCTF
b1,rgb,lsb,xy       .. text: "picoCTF{h1d1ng_1n_th3_b1t5}"
``` 
## Notas adicionales

## Referencias