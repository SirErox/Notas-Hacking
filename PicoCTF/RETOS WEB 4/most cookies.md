descripcion:
Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/99a50920a248ec37c39b8e3ab0af8789/server.py) [http://mercury.picoctf.net:18835/](http://mercury.picoctf.net:18835/)
solucion:
un reto asi esta mas complicado, porque hay que buscar una palabra secreta, que se uso para encriptar una cookie, y con flask-unsign le cambiamos a cualquier usuario a que sea admin... la palabra secreta "fortune" no importa que la pongas en la pagina, porque no eres admin... pero con la cookie firmada como admin mas facil...

despues use curl para obtener la bandera
picoCTF{pwn_4ll_th3_cook1E5_743c20eb}