#### Description

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/16/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/16/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/16/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

SOLUCION:

	Al descargar los ejercicios, vi que en el .py hace un chequeo con un documento que tiene encriptada la informacion, asi que como ya me da 7 valores, pues voy intentando uno por uno...

	al final pude acertar y obtener la contraseña:

	picoCTF{m45h_fl1ng1ng_2b072a90}