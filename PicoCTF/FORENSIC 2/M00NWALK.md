DESCRIPCION:
Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.

SOLUCION:
en una de las pistas nos pregunta, como es que le hacen para transmitir las imagenes de regreso a la luna... ya que el mensaje esta encriptado, no se escucha nada ni se ve nada

para este reto se sugiere instalar sstv decoder de github, un decodificador que usa la tecnologia de la transmision de imagenes...

despues de instalarlo solo tenemos que pasarle el mensaje al programa asi:

	sstv -d message.wav -o result.png 
solo detectara el tipo de codificacion, "scotty"...

despues veremos la bandera :

picoCTF{beep_boop_im_in_space}