descripcion:There is some interesting information hidden around this site [http://mercury.picoctf.net:55079/](http://mercury.picoctf.net:55079/). Can you find it?

---

solucion

en este reto es una suma de los retos web 1, es entrar en los diferentes archivos como css y js, despues es entrar en la parte de robots.txt

Llegando a la parte de robots.txt nos dice que como podemos acceder a un servidor apache... investigando resulta que hay una propiedad por asi decirlo...

http://mercury.picoctf.net:55079/.htaccess
 y despues nos dice que algo relacionado con una mac, crea sitios en una mac... asi que investigando resulta que hay un archivo para todas las mac, .DS_Store... 
asi que solo tenemos que reemplazarlo por .htaccess y tendremos las piezas

NOTA: LA BANDERA ESTA FRAGMENTADA, PERO EL RETO TE DA EL ORDEN DE LAS PIEZAS...
