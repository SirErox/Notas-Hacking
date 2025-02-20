Descripcion
Someone's commits seems to be preventing the program from working. Who is it?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/156/challenge.zip)

Solucion:

	Para este reto primero hice wget para tenerlo en la maquina virtual, luego le hice un unzip challenge.zip, y me meti a la carpeta de drop in...

	me fije que es casi igual que el anterior, asi que hice un git init para reactivar el repositorio, pero esta vez re-lei la descripcion del reto, y decidi aplicar el git log pero al archivo.py que esta en el directorio... y sorpresivamente esta la bandera:

picoCTF{@sk_th3_1nt3rn_d2d29f22}