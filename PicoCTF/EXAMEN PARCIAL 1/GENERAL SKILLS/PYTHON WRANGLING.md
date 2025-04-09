descripcion:
Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/ende.py) using [this password](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/pw.txt) to get [the flag](https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/flag.txt.en)?

SOLUCION
Primero haremos un wget en la maquina virtual, para trabajar mejor, ya que kali tiene python instalado por defecto

wget https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/ende.py
wget https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/pw.txt
wget https://mercury.picoctf.net/static/325a52d249be0bd3811421eacd2c877a/flag.txt.en

si analizamos el script ende.py vemos que trabaja con un archivo llamado pole.txt, pero no lo tenemos... asi que lo que tenemos encriptado es flag.txt.en, lo que contenga lo pasamos a un nuevo archivo llamado pole.txt

luego ejecutamos el codigo con: python ende.py -d pole.txt

nos pedira una contraseña, la cual esta dentro de pw.txt, asi que solo es darle un cat y poner esa contra al momento de ejecutar el codigo... y nos dara la bandera

picoCTF{4p0110_1n_7h3_h0us3_ac9bd0ff}