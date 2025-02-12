RETO: plumbing

Descripcion: 

	Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 4427`.

Traduccion:

	A veces necesitas manejar el procesamiento de datos afuera de un archivo, puedes encontrar una forma de mantener la salida de este programa y buscar la bandera? conectate a ...

Solucion: 

	Un ejercicio bastante similar a "what's a net cat?", ya desde un inicio nos dice que tenemos que conectarnos a tal servidor y capturar la salida de dicho programa...

	Como siempre usaremos una terminal, y usaremos una variante del comando nc

		Primero crearemos el archivo donde guardaremos la informacion, con el comando touch

	nc -v jupiter.challenges.picoctf.org 4427 < file.txt
	Lo que hace el comando es conectarse a la ip en tal puerto y lo que obtenga lo guardara en file.txt

	Pero como el ejercicio se llama plumbing, debemos procesar la salida directamente en el comando, con lo cual queda de la siguiente forma:
	nc jupiter.challenges.picoctf.org 442 < file.txt | egrep 'pico'
	Y con eso obtenemos la bandera:

	picoCTF{digital_plumb3r_5ea1fbd7}

	 
