descripcion:
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/3944a59474f9f676942282c50b9c3675/Forensics%20is%20fun.pptm)

solucion:
nos da una presentacion de powerpoint, pero estamos en forensic... asi que hay algo aqui que no cuadra...

primero le di un file y veo que esta bien el archivo, pero ahora le hago un UNZIP y veo que hay varios archivos y carpetas...

al urgar entre esos archivos encuentro uno que se llama hiden, y es una cadena separada por espacios en blanco....

para mayor comodidad quito esos espacios en blanco, puedo hacerlo con comando o a mano...

	tr -d " "  este comando quita los espacios en blanco 
	copio esa cadena en la consola y aplico el comando:

	echo "" | tr -d " " | base64 -d

si vemos la cadena sin espacios, parece base64... asi que decodificamos hay mismo y tenemos la bandera:

picoCTF{D1d_u_kn0w_ppts_r_z1p5}