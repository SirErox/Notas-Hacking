descripcion:
Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:17781/](http://mercury.picoctf.net:17781/)

solucion:

en este reto si tuve que mirar alguna solucion o writeup, para este reto si me estaba trabando, por alguna razon mozilla no me cargaba la pagina despues de modificar una cookie "name"

usando las herramientas sugeridas por el docente, y algo de logica, cambiando el navegador a google, pude ver que dependiendo del numero en esa cookie soltaba algo diferente...

en un video encontre un comando en consola de comandos... 

for i in {0..20}; do curl  -s .... ;done | grep pico

lo que hace es cambiar el valor de la cookie y checar si lo que tenemos de regreso es la bandera... si no lo es, cambia de valor y hace lo mismo, asi hasta intentar... es el 18 creo si no me falla

picoCTF{3v3ry1_l0v3s_c00k135_bb3b3535}