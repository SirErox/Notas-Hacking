descripcion.
We found this [file](https://mercury.picoctf.net/static/d0129ad98ba9258ab59e7700a1b18c14/tunn3l_v1s10n). Recover the flag.

solucion:
en este reto nos pasan un archivo que parece incompleto, cuando le aplicamos un file, solo nos dice que es data, asi que nos da una pista de que tendremos que completar ciertos bytes del archivo para poder verlo...

primero analizamos que es un BMP, pero hay que ver que usando hexeditor aparecen unos datos que no deberian...
BAD 

no es valido para un hexadecimal, no indica nada... asi que debemos cambiar esos por ciertos valores especificos...

despues de que se cambian esos valores debemos aumentar el alto de la imagen ya que esta algo reducida la imagen...


picoCTF{qu1t3_a_v13w_2020}