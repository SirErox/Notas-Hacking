descripcion:
Download the disk image and use `mmls` on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.[Download disk image](https://artifacts.picoctf.net/c/164/disk.img.gz)

solucion:
primero descargarmos la imagen en linux con wget, pero viene empaquetada disk.img.gz 

	gunzip disk.img.gz

nos dara un archivo disk.img, a este le aplicaremos un comando nuevo

	mmls disk.img

que nos dira como esta segmentada la imagen, y nos dice que encontremos el tamaño de la particion de linux...
	202752

despues nos conectaremos a un servidor para pasar ese numero y obtener la bandera..

nc saturn.picoctf.net 60934

picoCTF{mm15_f7w!}