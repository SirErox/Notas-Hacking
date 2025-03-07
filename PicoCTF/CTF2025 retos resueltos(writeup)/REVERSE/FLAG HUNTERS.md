Author: syreal

#### Description

Lyrics jump from verses to the refrain kind of like a subroutine call. There's a hidden refrain this program doesn't print by default. Can you get it to print it? There might be something in it for you.The program's source code can be downloaded [here](https://challenge-files.picoctf.net/c_verbal_sleep/349dec0af4fab981e8b730f4895232ce55148d80d74c4d0e14d36e00c7674558/lyric-reader.py).Connect to the program with netcat:`$ nc verbal-sleep.picoctf.net 59025`

Solucion:

Al inicio descargue el archivo y trate de entender el codigo, pero sin lograr nada decidi conectarme al servidor y ver de que se trataba el reto...

al intentar ingresar comandos o cualquier cosa de codigo, no me aceptaba nada... señal de que debia sortear el codigo o el filtrado de codigo...

En la parte del codigo pone .split ; con lo que ya nos da un punto de partida... pero para saber como sortearlo busque en internet como brincar esa seguridad...

me puse a experimentar con el codigo python local, y me fije que si ponia ; solo, se imprimia vacio, aqui ya tenemos una brecha de codigo...

Despues de varios intentos como ;REFRAIN, o ;RETURN 20, me fije que si aceptaba esos comandos, me salia otro texto diferente... asi que debia hacer que se imprimiera todo desde el inicio... por como estaba hecho el codigo..

;RETURN 0 y solo fue cuestion de esperar...
