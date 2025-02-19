Reto: RUNME.PY

#### Description

Run the `runme.py` script to get the flag. Download the script with your browser or with `wget` in the webshell.[Download runme.py Python script](https://artifacts.picoctf.net/c/34/runme.py)

Solucion:

No tiene chiste, en este reto es solo descargar el archivo y ejecutarlo con python, se recomienda usar una terminal de linux, ya que trae el python por defecto
```
(kali㉿kali)-[~/Downloads]
└─$ wget https://artifacts.picoctf.net/c/34/runme.py  
--2025-02-17 19:28:04--  https://artifacts.picoctf.net/c/34/runme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.55.61, 3.161.55.64, 3.161.55.100, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.55.61|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 270 [application/octet-stream]
Saving to: ‘runme.py’

runme.py         100%[=======>]     270  --.-KB/s    in 0s      

2025-02-17 19:28:05 (420 MB/s) - ‘runme.py’ saved [270/270]

                                                                 
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 runme.py 
picoCTF{run_s4n1ty_run}
```