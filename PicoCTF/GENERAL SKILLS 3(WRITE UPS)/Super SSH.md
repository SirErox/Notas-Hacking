Reto:Super SSH

#### Description

Using a Secure Shell (SSH) is going to be pretty important.

Additional details will be available after launching your challenge instance.

Solucion:
	El problema ya te dice que tienes que hacer una vez que lanzas la instancia... conectarte usando ssh a cierto servidor usando el puerto x...

Aunque es demasiado obvia la solucion, hay un parametro que no usamos en esa conexion y es -2 que es decirle a la consola usar la version 2 del ssh, ya que por defecto usamos la primera version
```
ssh -2 ctf-player@titan.picoctf.net -p 63324
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_3e293eea}
Connection to titan.picoctf.net closed.
```