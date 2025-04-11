DESCRIPCION:
Why search for the flag when I can make a bookmarklet to print it for me?

SOLUCION:
Cuando entramos al sitio nos muestra como parte de un codigo, y ese codigo podemos ejecutarlo en la consola de chrome... con lo cual nos suelta la bandera

codigo: 

	        javascript:(function() {
            var encryptedFlag = "àÒÆÞ¦È¬ëÙ£Ö�ÓÚåÛÑ¢ÕÓË¨Ë�Ó�§Èí";
            var key = "picoctf";
            var decryptedFlag = "";
            for (var i = 0; i < encryptedFlag.length; i++) {
                decryptedFlag += String.fromCharCode((encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256);
            }
            alert(decryptedFlag);
        })();

picoCTF{p@g3_turn3r_e8b2d43b}