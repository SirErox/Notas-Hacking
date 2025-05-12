descripcion:

	The [numbers](https://jupiter.challenges.picoctf.org/static/f209a32253affb6f547a585649ba4fda/the_numbers.png)... what do they mean?

solucion:
	
	En este caso nos dan una imagen, si la abrimos vemos unos numeros... con la forma de la bandera... intuimos como empieza y nos da la idea de que es una sustitucion, que la A es tal valor y asi...
	
	A esta sustitucion se le conoce como AIZ26, lo que hace es tomar la posicion de la letra segun el alfabeto y pone el numero en su lugar, asi que usamos cyberchef para esta conversion...
	https://gchq.github.io/CyberChef/#recipe=A1Z26_Cipher_Decode('Space')&input=MTYgOSAzIDE1IDMgMjAgNiAyMCA4IDUgMTQgMjEgMTMgMiA1IDE4IDE5IDEzIDEgMTkgMTUgMTQ

	16 9 3 15 3 20 6 {20 8 5 14 21 13 2 5 18 19 13 1 19 15 14}
	picoctf{thenumbersmason}