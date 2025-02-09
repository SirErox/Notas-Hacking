RETO: First Grep

Descripción:

	Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file)? This would be really tedious to look through manually, something tells me there is a better way.

Traducccion:

	Puedes encontrar la bandera en ...? esto podria ser realmente tedioso de mirar manualmente, algo me dice que hay una mejor forma

Solución:

	Para esto primero debemos descargar ese archivo, use la pista del reto y me paso a un tutorioal, y como bien dice en el nombre del reto, es usar un GREP, que es un comando de linux, para esto usare la maquina virtual de kali.

	le pasare el archivo a la maquina y abrire una terminal para poder trabajar con el archivo...
	Para poder trabajar con el archivo mas facil, pasaremos la informacion a un archivo de texto con cat... el comando seria:
	cat files > grep.txt
	de esta forma puedo hacer diferentes pruebas con la informacion del archivo sin alterarlo
	Despues intentare con "egrep -n 'flag' grep.txt"
	Al darme cuenta que no me solto nada el comando, me percate que ese no es el formato que buscamos...
	si no "pico..." asi que cambie flag por pico en el comando y obtuve la bandera
	picoCTF{grep_is_good_to_find_things_f77e0797}
