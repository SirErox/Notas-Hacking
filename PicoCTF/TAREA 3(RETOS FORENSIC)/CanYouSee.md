descripcion:

	How about some hide and seek?Download this file [here](https://artifacts.picoctf.net/c_titan/129/unknown.zip).
solucion:

	Al desempaquetar el archivo solo deja una imagen sin errores internos, asi que aplico "exiftool ukn.png" y en una parte hay una cadena como codificada, asi que como es costumbre, esta en base64

	echo cGljb0NURntNRTc0RDQ3QV9ISUREM05fYjMyMDQwYjh9Cg== | base64 -d

	picoCTF{ME74D47A_HIDD3N_b32040b8}