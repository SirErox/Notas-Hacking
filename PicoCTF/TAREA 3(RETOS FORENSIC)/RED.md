descripcion:
	
	RED, RED, RED, REDDownload the image: [red.png](https://challenge-files.picoctf.net/c_verbal_sleep/831307718b34193b288dde31e557484876fb84978b5818e2627e453a54aa9ba6/red.png)

solucion:

	Una imagen completamente roja, si aplicamos un exiftool  veremos un poema incrustado... no da pista pero es interesante...

	si despues le aplicamos un zsteg, veremos que sale una cadena que se repite varias veces, dicha cadena esta codificada en base64, asi que copiamos hasta los primeros 2 = y decodificamos...

echo cGljb0NURntyM2RfMXNfdGgzX3VsdDFtNHQzX2N1cjNfZjByXzU0ZG4zNTVffQ== | base64 -d

	picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}