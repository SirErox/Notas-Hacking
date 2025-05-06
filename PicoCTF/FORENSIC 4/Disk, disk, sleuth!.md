descripcion:
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/2f998eee12730cf5766624681212a441/dds1-alpine.flag.img.gz)

solucion:
ya una vez que tenemos el archivo en el entorno de linux, tenemos que desempaquetarlo del .gz
	
	gunzip dds1-alpine.flag.img.gz

despues nos dejara la imagen... pero ahora debemos buscar la bandera, y para hacerlo mas conveniente, usaremos la tecnica de pipeing con buscar cadenas

	srch_strings dds1-alpine.flag.img | grep pico

sy en poco tiempo deberiamos tener la bandera
	picoCTF{f0r3ns1c4t0r_n30phyt3_267e38f6}