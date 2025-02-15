Reto: ### Magikarp Ground Mission

Descripcion:
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `b60940ca`

Additional details will be available after launching your challenge instance.

Hints: Finding a cheatsheet for bash would be really helpful!
solucion:

primero me conecte a la instancia para ver que me decia
```
(kali㉿kali)-[~/files]
└─$ ssh ctf-player@venus.picoctf.net -p 52739
The authenticity of host '[venus.picoctf.net]:52739 ([3.131.124.143]:52739)' can't be established.
ED25519 key fingerprint is SHA256:P1f6h95BrSVnJbm2AKhphfHHGEyAeThib/rN/AwKs24.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? Y
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added '[venus.picoctf.net]:52739' (ED25519) to the list of known hosts.
ctf-player@venus.picoctf.net's password: 
Permission denied, please try again.
ctf-player@venus.picoctf.net's password: 
Welcome to Ubuntu 18.04.5 LTS (GNU/Linux 5.4.0-1041-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage
This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

ctf-player@pico-chall$ dir
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt 
picoCTF{xxsh_

//aqui decidi abrir ambos archivos al mismo tiempo y vi que decia de iral directorio raiz
ctf-player@pico-chall$ cat 1of3.flag.txt instructions-to-2of3.txt 
picoCTF{xxsh_
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cat  instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ ls -la
total 16
drwxr-xr-x 1 ctf-player ctf-player 4096 Mar 16  2021 .
drwxr-xr-x 1 ctf-player ctf-player 4096 Feb 15 17:56 ..
-rw-r--r-- 1 ctf-player ctf-player   14 Mar 16  2021 1of3.flag.txt
-rw-r--r-- 1 ctf-player ctf-player   56 Mar 16  2021 instructions-to-2of3.txt
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ dir
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var

//Aqui vi el documento de texto, pero decidi abrir ambos, y vi que la bandera estaba segmentada... solo era seguir las instrucciones

ctf-player@pico-chall$ ls
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cat 2of3.flag.txt instructions-to-3of3.txt 
0ut_0f_\/\/4t3r_
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ cd ..
ctf-player@pico-chall$ dir
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cd ..
ctf-player@pico-chall$ dir
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cat file.txt
cat: file.txt: No such file or directory
ctf-player@pico-chall$ cd home
ctf-player@pico-chall$ dir
ctf-player
ctf-player@pico-chall$ cat ctf-player/
cat: ctf-player/: Is a directory
ctf-player@pico-chall$ cd ctf-player/
ctf-player@pico-chall$ dir
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt 
c1754242}
ctf-player@pico-chall$ Connection to venus.picoctf.net closed by remote host.
Connection to venus.picoctf.net closed.
```
	
	Despues juntamos la parte de los .txt y tenemos la bandera
	picoCTF{xxsh_0ut_0f_\/\/4t3r_c1754242}
