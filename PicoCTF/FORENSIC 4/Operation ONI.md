Descripcion:
Download this disk image, find the key and log into the remote machine.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

solucion:

despues de descarga la imagen y cargarla en autopsy, urgando en el directorio root veo que hay una carpeta .ssh, y en el historial vemos que hizo unas llaves para entrar a un servidor...
asi que si queremos entrar, debemos copiar esas llaves tal y como estan, con los permisos incluidos...

en la imagen la llave nomas tiene permisos para el usuario actual, pero cuando la pasamos para usar nosotros, tiene varios.. asi que usamos 

	chmod 600 id...

y despues nos conectamos al servidor, si todo esta bien, no pedira contraseña y podremos entrar...

picoCTF{k3y_5l3u7h_b5066e83}