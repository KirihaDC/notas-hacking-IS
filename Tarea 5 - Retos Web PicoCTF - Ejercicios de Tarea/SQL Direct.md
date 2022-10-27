# SQL Direct

## Objetivo
¡Conéctate a este servidor PostgreSQL y encuentra la bandera!`psql -h saturn.picoctf.net -p 49327 -U postgres pico`La contraseña es`postgres`

## Solucion
``` shell
┌──(kiriha㉿kali)-[~]
└─$ psql -h saturn.picoctf.net -p 49327 -U postgres pico
Contraseña para usuario postgres: 
psql (14.4 (Debian 14.4-1+b1), servidor 14.2 (Debian 14.2-1.pgdg110+1))
Digite «help» para obtener ayuda.

pico-# \t
Mostrar sólo filas está activado.
pico-# \l
 pico      | postgres | UTF8         | en_US.utf8 | en_US.utf8 | 
 postgres  | postgres | UTF8         | en_US.utf8 | en_US.utf8 | 
 template0 | postgres | UTF8         | en_US.utf8 | en_US.utf8 | =c/postgres          +
           |          |              |            |            | postgres=CTc/postgres
 template1 | postgres | UTF8         | en_US.utf8 | en_US.utf8 | =c/postgres          +
           |          |              |            |            | postgres=CTc/postgres

pico-# \dt
 public  | flags  | tabla | postgres
         
pico=# select * from flags;
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia

pico=#
```

## Notas adicionales

## Referencias