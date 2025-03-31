Descripcion:
Can you find the flag on this website.

Additional details will be available after launching your challenge instance.

solucion:

En este reto veremos mas a fondo lo que es el sqlite, una version reducida de sql
Primero nos pide ingresar al sitio, asi que haremos lo mismo que en el reto IRISH-NAME-REPO 1, sortearemos tanto el usuario como la contraseña

Despues de que entremos tendremos que buscar esa tabla sin ver en la base de datos, no sabemos como se llama la tabla... ni donde esta ubicada... asi que haremos un union...

	'union SELECT sql,2,3 from sqlite_master;
	
NOTA: Para inyeccion sql es usar ' al inicio del comando y acabar con ;

nos dara los comandos que usaron para crear las tablas, y aqui veremos que hay una tabla con campo FLAG... tenemos que ver esa tabla...

	'union select id,flag,3 from more_table;

picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_c8ee9477}