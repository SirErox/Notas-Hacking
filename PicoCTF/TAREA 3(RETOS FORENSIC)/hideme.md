descripcion:

	Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/262/flag.png).

solucion:

	Reto bastante parecido al de la muñeca rusa, esta vez ocupamos el comando binwalk
	primero le hice un binwalk sin la opcion de -e y me dice que hay un comprimido en la imagen, asi que le puse la opcion -e y me meto al folder que suelta el comadno
		"binwalk -e flag.png"

	adentro hay una carpeta que se llama secret, asi que entramos y es la bandera...

	picoCTF{Hidding_An_imag3_within_@n_imag9e_82101824}
	