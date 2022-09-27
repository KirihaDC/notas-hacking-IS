# Nice netcat

## Objetivo 
Descripción:
Hay un buen programa con el que puedes hablar usando este comando en un shell: `$ nc mercury.picoctf.net 35652`, pero no habla inglés...

Sugerencias:
Puedes practicar el uso de netcat con este problema de picoGym: [¿qué es un netcat?](https://play.picoctf.org/practice/challenge/34)

Puedes practicar la lectura y escritura ASCII con este problema de picoGym: [Vamos a calentar](https://play.picoctf.org/practice/challenge/22)

## Solución 
``` shell
┌──(kiriha㉿kali)-[~]
└─$ nc mercury.picoctf.net 35652
112
105
99
111
67
84
70
123
103
48
48
100
95
107
49
116
116
121
33
95
110
49
99
51
95
107
49
116
116
121
33
95
57
98
51
98
55
51
57
50
125
10

picoCTF{g00d_k1tty!_n1c3_k1tty!_9b3b7392}
```

## Notas
Para entrar recuerda que debes de poner el servidor y el puerto, similar a los retos bandit:
nc mercury.picoctf.net 35652
Tambien podemos usar herramientas externas para resolver los retos, como para convertir los ASCII a TEXTO

## Referencias
[nc](https://linux.die.net/man/1/nc)
[convertidor de ASCII A TEXTO](https://es.rakko.tools/tools/76/)