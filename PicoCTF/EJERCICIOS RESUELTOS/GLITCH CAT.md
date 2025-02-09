RETO: GLITHC CAT

Descripción:

	Our flag printing service has started glitching!
	Additional details will be available after launching your challenge instance.

Traduccion:

	Nuestro servicio de impresion de banderas ha empezado a buguearse!
	Detalles adicionales seran disponibles despues de lanzar tu instancia del reto

Solución:

	Al ejecutar la instancia nos da un comando para poder conectarnos "$ nc saturn.picoctf.net 62084"

	Lo primero que hice fue capturar todo en un txt, asi que use < glitch.txt para despues analizarlo...

	'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'

	La bandera esta incompleta... pero algo es familiar... vemos que tiene simbolos de + y luego usa como una funcion y se le pasa el valor en hexadecimal...

	Si revisamos la funcion chr, regresa un caracter en funcion del integer que le pasemos, pero aqui se le estan pasando hexadecimales...

	Converti todos los hexa en decimales primero

	chr(57) + chr(99) + chr0(52) + chr(50) + chr(97) + chr(52) + chr(53) + chr(100)

	En las pistas del reto, nos dice que es una salida valida de python o algo relacionado, asi que ya con los numeros formateados puse la linea en python...

	picoCTF{gl17ch_m3_n07_' + chr(57) + chr(99) + chr0(52) + chr(50) + chr(97) + chr(52) + chr(53) + chr(100) 
	
	'picoCTF{gl17ch_m3_n07_9c42a45d}'

	Tambien podemos poner la linea original con los hexa en python y nos dara la bandera completa... (me dio curiosidad y funciono... jajajajajaja)