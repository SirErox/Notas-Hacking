Reto: ### Wave a flag

Descripcion:
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...

Hints:
	1 This program will only work in the webshell or another Linux computer.
	2 To get the file accessible in your shell, enter the following in the Terminal prompt: $ wget https://mercury.picoctf.net/static/cfea736820f329083dab9558c3932ada/warm
	3 Run this program by entering the following in the Terminal prompt: $ ./warm, but you'll first have to make it executable with $ chmod +x warm
	4 -h and --help are the most common arguments to give to programs to get more information from them!
	5 Not every program implements help features like -h and --help.

Solucion: primero empiezo por descargar el programa con wget, y luego se me ocurrio darle un file para ver que tipo de archivo es... un elf64 ejecutable...

Asi que le di un cat y sorpresa... no tarde en identificar la bandera a plena vista...

Aunque si se seguimos las pistas, le di un chmod +x al programa y lo ejecute, luego luego me dice que le pase un -h para mas informacion y me da la bandera como si nada...
````
──(kali㉿kali)-[~/Downloads]
└─$ ./warm           
Hello user! Pass me a -h to learn what I can do!
                                                                                                                                                                       
┌──(kali㉿kali)-[~/Downloads]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_30e77291}
```