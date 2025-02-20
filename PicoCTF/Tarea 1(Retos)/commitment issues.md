Descripcion:
	I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/75/challenge.zip)

Solucion:

	Para este reto descargue el archivo y al hacer un unzip -l challenge.zip veo que es un repositorio .git

	Asi que para este reto se ocupa conocer algunos comandos basicos del git, pero algo dificiles de reconocer...

	Primero hacemos un GIT INIT donde esta el .git, debe aparecernos que esta rehabilitado el repositorio, y despues podemos ver que commits se han hecho con git log...

	Vemos que hizo un commit que dice create flag... y tenemos que borrar ese cambio, asi que para eso hacemos "git checkout <ID mostrado en git log>" y nos dira que se revirtieron los cambios... 

	Se me pasaba comentar que al momento de desempaquetar el archivo, hay un archivo que se llama message.txt... que antes de aplicar el comando checout, no aparece la bandera... pero despues de que hacemos el comando, aparecera la bandera...

picoCTF{s@n1t1z3_9539be6b}