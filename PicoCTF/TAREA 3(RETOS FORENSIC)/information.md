descripcion:

	Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg)

solucion:

	En este reto hay una pista que nos dice que como vemos los detalles a fondo de la imagen, para esto debemos usar una distro linux o kali, ocupamos el comando exiftools...

		exiftool cat.jpg


	una vez que nos de la metadata del archivo vemos que en la parte de la licencia no corresponde lo que dice... parece codificado, y por experiencia parece ser base64, asi que lo ponemos en la misma consola

	echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d 
	y nos dara la bandera
	
	picoCTF{the_m3tadata_1s_modified}