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

//Revisar notas
```

## Notas
Podemos usar grep para obtener la contraseña o abrir el archivo de manera manual y poder acceder a la bandera correspondiente.

Nota del codigo: No pude sacar la bandera por errores que me da la maquina virtual al momento de arrancarlo pero la solucion si es la de arriba, cuando pueda hacer funcionar la maquina virtual actualizare los retos para subir las banderas a mis codigos de obsidian y al picoCTF para que se queden registradas de igual forma en la plataforma y salgan los puntos en mi perfil.

## Referencias
 [Descargar bandera](https://mercury.picoctf.net/static/a5683698ac318b47bd060cb786859f23/flag)