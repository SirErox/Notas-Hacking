DESCRIPCION:

Cookie Monster has hidden his top-secret cookie recipe somewhere on his website. As an aspiring cookie detective, your mission is to uncover this delectable secret. Can you outsmart Cookie Monster and find the hidden recipe?You can access the Cookie Monster [here](http://verbal-sleep.picoctf.net:60118/) and good luck

SOLUCION:
AL entrar al sitio nos pide un usuario y contraseña, le di los datos basicos "admin" y "admin", y me dice que accesso denegado, que el monstruo no necesita contraseña, si no galletas

y nos dice una pista "has checado tus galletas?" con lo cual usando un inspector de cookies, veo una que se llama "secret recipe"

cGljb0NURntjMDBrMWVfbTBuc3Rlcl9sMHZlc19jMDBraWVzX0E5NjRBMTM0fQ%3D%3D

al ver esta cadena noto que es una encryptacion, pero no se que tipo, ya que %3D me confunde, asi que hago uso de cyberchef  https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&oeol=CR y pongo la formula para decodificar de base64...

al momento que ingreso la formual, se decodifica y sale la bandera

picoCTF{c00k1e_m0nster_l0ves_c00kies_A964A134}