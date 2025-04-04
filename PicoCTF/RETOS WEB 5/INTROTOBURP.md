DESCRIPCION:
Try [here](http://titan.picoctf.net:61122/) to find the flag

SOLUCION:
BURP NO SUPE USARLO, YA QUE NO PUDE VER BIEN LOS PAQUETES SEGUI USANDO MOZILLA FIREFOX

en mozilla una ves que carguemos la pagina y veamos como se comporta, vemos que pide 2fa, pero no valida ni los datos antes de enviarlos para el registro

asi que inspeccionando el codigo vemos que pone una variable otp=xxxx... un poco raro en codigo html

asi que solo borramos esa parte y reenviamos la solicitud, despues se veera en la respuesta de la misma consola


picoCTF{#0TP_Bypvss_SuCc3$S_b3fa4f1a}