descripcion:
Can you abuse the banner?

Additional details will be available after launching your challenge instance.

solucion:
hay 2 conexiones, la primera solo nos dara una contraseña para conectarnos a la segunda usando nc

una vez que entramos nos pide unos detalles, como que DEFCON es la conferencia de seguridad a nivel mundial mas importante y quien fue el primer hacker en realizar llamadas gratis, despues nos deja entrar al servidor

Urgando entre los archivos, ejecute un comando ls -la /root y vi el archivo flag.txt

nos mencionaba al inicio algo de un symlink, es un enlace simbolico, asi que usaremos eso y los permisos que tenemos...

borramos en banner.txt y creamos el enlace simbolico con ese nombre para que no sospeche el script

ln -s /root/flag.txt banner

lo que hacemos es que el enlace simbolico abra ese archivo cuando se ejecute... asi que saliendo del servidor y ejecutando denuevo la entrada, nos dara la bandera:

picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_218ef5d6}

