# Obedient Cat

## Objetivo 
Descripción:
Este archivo tiene una bandera a plena vista (aka "in-the-clear"). [Descargar bandera](https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag).

Sugerencias:
Cualquier sugerencia sobre cómo ingresar un comando en la Terminal (como la siguiente), comenzará con un '$'... todo lo que esté después del signo de dólar se escribirá (o copiará y pegará) en su Terminal.

  
Para acceder al archivo en su shell, ingrese lo siguiente en el indicador de Terminal: $ wget https://mercury.picoctf.net/static/33996e32dce022205a6a36f69aba56f0/flag
$ man cat

## Solución 
``` shell
//que no se te olvide ir a descargas
┌──(kiriha㉿kali)-[~]
└─$ cd Descargas 
                                                                 
┌──(kiriha㉿kali)-[~/Descargas]
└─$ grep 'picoCTF' flag

picoCTF{s4n1ty_v3r1f13d_2aa22101}
```

## Notas
Podemos usar grep para obtener la contraseña o abrir el archivo de manera manual y poder acceder a la bandera correspondiente.

## Referencias
 [Descargar bandera](https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag)