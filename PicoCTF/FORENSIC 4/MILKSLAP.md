descripcion:
🥛

solucion:
Pareciera reto de la categoria web pero es forense y aqui es analizar una imagen... asi que primero tenemos que sacar esa imagen que se mueve conforme movemos el mouse

	http://mercury.picoctf.net:29522/concat_v.png

investigando en la pagina, llegamos a la hoja de estilos y solo es poner eso para ver que es un png muy largo...

despues de tenerlo en un entorno linux tendremos que usar zsteg, una herramienta para este tipo de casos de steganografia

	gem install zsteg

despues es aplicar el comando 

zteg concat_v.png

y debe soltarte la bandera, a mi en lo personal me dio muchos problemas...

picoCTF{imag3_m4n1pul4t10n_sl4p5}