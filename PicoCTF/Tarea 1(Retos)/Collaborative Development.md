Descripcion:
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/70/challenge.zip)

solucion:

Similar a blame game, pero esta vez tenemos varias ramas de trabajo... y aparentemente tenemos la bandera en segmentos... asi que ya una vez desempaquetado el archivo y reinicializado el repo... ocupamos un comando que nos permita ver las ramas de trabajo, git branch -a  y vemos que dice feature... 

Tenemos que cambiar a cada una de esas ramas en orden numerico, asi que le damos un git checkout feature... y nos cambia a la rama de trabajo, como el archivo flag.py cambia... debemos hacer un cat flag.py y sacar la parte de la bandera, para despues pegarla... o ver la manera de concatenar todos los cat y sacar la bandera:

	picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}