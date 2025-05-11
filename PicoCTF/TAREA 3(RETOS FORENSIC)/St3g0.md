descripcion:
	
	Download this image and find the flag.

	- [Download image](https://artifacts.picoctf.net/c/216/pico.flag.png)

solucion:

	Primero analize la imagen con "file pico.flag.png" y todo estaba bien, tambien analize con exiftools y nada fuera de lo comun...

	El nombre del reto nos dice que es de steganografia, asi que ocupamos la herramienta ZSTEG, "zsteg pico.flag.png" y saldra la bandera

	picoCTF{7h3r3_15_n0_5p00n_a1062667}