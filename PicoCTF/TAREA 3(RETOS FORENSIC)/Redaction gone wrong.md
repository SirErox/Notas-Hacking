descripcion:

	Now you DON’T see me.This [report](https://artifacts.picoctf.net/c/84/Financial_Report_for_ABC_Labs.pdf) has some critical data in it, some of which have been redacted correctly, while some were not. Can you find an important key that was not redacted properly?

solucion:

	Al descargar el archivo pdf, intento hacerle un cat con un grep para ver si puedo sacar la bandera, pero no funciono, asi que intento abrirlo "open archivo.pdf"

	y al abrirlo solo seleccione el texto completo y se ve la bandera a plena vista...

	picoCTF{C4n_Y0u_S33_m3_fully}