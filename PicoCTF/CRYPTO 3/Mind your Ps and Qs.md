Descripcion:

	In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values)

solucion:

	Para este reto se ocupo la herramienta RsaCtfTool, que ya nos ayuda con los pasos para resolver los retos, solo tenemos que pasarle los datos necesarios...

	el comando usado fue:
	RsaCtfTool -n 1311097532562595991877980619849724606784164430105441327897358800116889057763413423 -e 65537 --decrypt 861270243527190895777142537838333832920579264010533029282104230006461420086153423 

	y en poco tiempo tendremos el texto desifrado
	picoCTF{sma11_N_n0_g0od_13686679}