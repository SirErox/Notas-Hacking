descripcion: I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/74274b96fe966126a1953c80762af80d/whitepages.txt) is all blank!

solucion:
al descargar el archivo .txt y hacerle un file, nos dice que contiene caracteres UNICODE, pero al ver detenidamente, contiene 2 tipos de espacios... y aunque "este vacio" no lo esta, si le ponemos un cat, se imprimen lineas vacias...

Ocuparemos pwntools, una libreria muy conocida en el ambito de hacking y de eventos CTF, para instalarla use:

pipx install pwntools

despues tenemos que pasarle el archivo txt como binario para quitar esos espacios en blanco que se imprimen pero no se ven...

ahora tendremos que crear un archivo donde estaremos modificando ese archivo...

	from pwn import *
	file=open("whitepages.txt","rb")
	data=bytearray(file.read())
	data=data.replace(b'\xe2\x80\x83',b'0')
	data=data.replace(b'\x20',b'1')
	data=data.decode('ascii')
	data=unbits(data)

	print(data)

este programa lee los bytes del archivo, reemplazamos las cadenas raras por 0, y los espacios por 1, luego decodificamos del ascii y sale la bandera

picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}