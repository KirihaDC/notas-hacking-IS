# Irish-Name-Repo 3

## Objetivo 
Hay un sitio web seguro en https://jupiter.challenges.picoctf.org/problem/29132/ (enlace) o http://jupiter.challenges.picoctf.org:29132. ¡Intenta ver si puedes iniciar sesión como administrador!

## Solución 
Inyectamos el siguiente codigo SQL en la parte de usuario y password para ver como actua el sistema codificando nuestra carga util: password'be'1'='1

# Logged in!

Your flag is: picoCTF{3v3n_m0r3_SQL_06a9db19}

# Logged in!

Your flag is: picoCTF{s0m3_SQL_c218b685}

## Notas
Al probar inyecciones de codigo podemos ver y evaluar el comportamiento de la pagina a la hora de querer acceder a alguna parte del sistema.

## Referencias