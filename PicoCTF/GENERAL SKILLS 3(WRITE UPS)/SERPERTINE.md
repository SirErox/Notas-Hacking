Find the flag in the Python script![Download Python script](https://artifacts.picoctf.net/c/36/serpentine.py)

Solucion:
	Descargue el archivo y le di un cat, mi vista se fijo en una funcion conocida, que decia print_flag... con lo cual es lo mismo del pw crack 1, analizando el codigo hay un menu basico... pero en donde aparece la opcion de imprimir bandera... no se llama la funcion... asi que solo modifique el archivo para llamar a la funcion y salio la bandera:


picoCTF{7h3_r04d_l355_7r4v3l3d_aa2340b2}
