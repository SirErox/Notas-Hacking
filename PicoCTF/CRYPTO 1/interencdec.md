descripcion:

	Can you get the real meaning from this file.Download the file [here](https://artifacts.picoctf.net/c_titan/1/enc_flag).

solucion:

	al descargar el archivo y ver el contenido sale una cadena codificada en base64, por los == al final de la codificacion, despues sale una cadena con b'' pero eso es para confundir, ya que tenemos una cadena en base4 dentro... asi que la decodificamos de nuevo y ahora solo es aplicar ROT13 con cyberchef para obtener la respuesta
	https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,19)&input=d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2xoNjBsMDBp
	
	picoCTF{caesar_d3cr9pt3d_ea60e00b}