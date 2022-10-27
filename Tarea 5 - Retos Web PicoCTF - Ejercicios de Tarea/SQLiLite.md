# SQLiLite

## Objetivo
¿Puedes iniciar sesión en este sitio web?Intente iniciar sesión [aquí](http://saturn.picoctf.net:49418/) .
## Solucion
Para darle solucion a este problema tenemos que usar el inspector del navegador para poder acceder a las acciones que que se realizan a la hora de probar los usuarios y contraseñas, para acceder a la contraseña debemos poner admin' -- en usuario y password ya que es una de las sentencias que se utiliza en SQL, de esta forma a la hora de darle en sumit nos dara el mismo error pero en el inspector podremos ver la bandera en unos de los comentarios:
picoCTF{L00k5_l1k3_y0u_solv3d_it_9b0a4e21}
## Notas adicionales

## Referencias