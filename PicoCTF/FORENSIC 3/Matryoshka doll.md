Descripcion:
Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/5ef2e9103d55972d975437f68175b9ab/dolls.jpg)

solucion:

como dice el nombre del reto... es algo dentro de ese algo, asi sucesivamente... 

en este caso tenemos una imagen, que se puede abrir normalmente, pero adentro tiene un comprimido y una carpeta con mas cosas... asi que usaremos binwalk...

un comando que nos permite sacar esos archivos... primero aplicamos binwalk -e dolls.jpg y lo que salga tendremos que aplicar lo mismo

hasta que salga un archivo "flag.txt"



picoCTF{e3f378fe6c1ea7f6bc5ac2c3d6801c1f}