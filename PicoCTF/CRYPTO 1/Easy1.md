descripcion:

	The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.

solucion:

	Lo que tenemos que resolver o desencriptar es SOLVECRYPTO, que dada la tabla, tenemos que ir letra por letra...
	la primera letra debemos encontrarla en las filas, despues avanzar hasta la primera letra U, y el nombre de la columna es nuestra letra final....

	Tambien podemos usar: con one time pad
	https://www.dcode.fr/cipher-identifier
	picoCTF{CRYPTOISFUN}