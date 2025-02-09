RETO: NICE NETCAT

Descripcion:
	
	There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 22902`, but it doesn't speak English...

Traduccion:

	Hay un buen programa con el cual puedes hablar usando el comando..., pero el no habla ingles...

Solucion:

	Primero ejecute el comando que me da el ejercicio y me da puros decimales pero en lista... con lo cual es algo curioso, al ver los numeros veo que algunos se repiten... como si se tratase de algun texto oculto(la bandera).

	Asi que la salida la meti a un archivo txt, despues me percate que puedo usar python para convertir esos numeros en ascii, asi que hice un archivo con una lista de esos numeros

	![[Pasted image 20250209135114.png]]
	(imagen añadida)
			Lo que hace el script es recorrer la lista con los valores y por cada uno, lo va a convertir a Char y lo imprime en pantalla
	Al ejecutar el script en IDLE de python me da la bandera correctamente! 
	picoCTF{g00d_k1tty!_n1c3_k1tty!_d3dfd6df}
	La bandera sale de manera vertical, pero no es problema acomodarla