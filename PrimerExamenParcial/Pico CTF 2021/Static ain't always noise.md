# Static ain't always noise

## Objetivo 
Descripción:
¿Puedes mirar los datos en este binario: [estático](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static) ? ¡ Este [script BASH](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh) podría ayudar!

## Solución 
```` shell                                             
┌──(kiriha㉿kali)-[~/Descargas]
└─$ ls    
Addadshashanammu.zip  ltdis.sh                  static.ltdis.x86_64.txt  warm.1
file                  static                    strings
flag                  static.ltdis.strings.txt  warm
                                                                                
┌──(kiriha㉿kali)-[~/Descargas]
└─$ unzip Addadshashanammu.zip                   
Archive:  Addadshashanammu.zip
   creating: Addadshashanammu/
   creating: Addadshashanammu/Almurbalarammi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/
   creating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/
  inflating: Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet  
                                                                                
┌──(kiriha㉿kali)-[~/Descargas]
└─$ cd Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku 
                                                                                
┌──(kiriha㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ file fang-of-haynekhtnamet 
fang-of-haynekhtnamet: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=5fffe70019957f0a27a70bb886b2cfb9f9b21d6e, not stripped
                                                                                
┌──(kiriha㉿kali)-[~/…/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku]
└─$ ./fang-of-haynekhtnamet 
ZAP! picoCTF{l3v3l_up!_t4k3_4_r35t!_76266e38}
````

## Notas
Debes tomar en cuenta los permisos, aveces solo basta con tener los permisos para pasar de nivel y tener acceso a algunas funciones para poder resover el reto y sacar la bandera y debemos descargar los achivos correspondientes.

## Referencias
 [linck del static](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/static)
 [link del script](https://mercury.picoctf.net/static/7495259e963bd5b67d0fb8b616652618/ltdis.sh)