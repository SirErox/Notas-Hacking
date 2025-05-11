descripcion:

	The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the information from this strange file?Download the suspicious file [here](https://artifacts.picoctf.net/c_titan/97/flag2of2-final.pdf).

solucion:

	En este reto solo nos dan un archivo pdf, si lo abrimos encontramos una parte de la bandera, pero si le damos un "file archivo.pdf" nos dice que es una imagen... cosa que no coincide..

	asi que creamos una copia con extencion .png "cp archivo.pdf flag.png" abrimos ese nuevo archivo y tenemos la primera parte de la bandera, solo juntamos las partes y listo
	
	picoCTF{f1u3n7_1n_pn9_&_pdf_724b1287}