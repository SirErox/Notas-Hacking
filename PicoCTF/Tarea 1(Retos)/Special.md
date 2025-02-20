#### Description

Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM)Start your instance to see connection details.

Additional details will be available after launching your challenge instance.

Solucion:
	Al conectarme al reto me percato que los comandos que pongo por alguna razon no funiconan... intente buscar diferente informacion acerca de lo shell, pero ninguna se parecia...

Asi que encontre esta informacion del writeup respectivo
		
	https://github.com/snwau/picoCTF-2023-Writeup/blob/main/General%20Skills/Special/Special.md

El tipo dice que intento encerrando en doble parentesis el comando a ejecutar, pero de 1 palabra... intente con el ls y me dio blargh, indicando que era un directorio... 

Asi que intente  dar un cat a ese directorio, asumi que la bandera estaria en "flag.txt" dentro de este directoro blargh... y si, salio la bandera:

```
ssh -p 60455 ctf-player@saturn.picoctf.net   
The authenticity of host '[saturn.picoctf.net]:60455 ([13.59.203.175]:60455)' can't be established.
ED25519 key fingerprint is SHA256:tJ0wuU5yBvNO/FrkHmR9iY36VJClMhKV+Hq2sxqKFmg.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:60455' (ED25519) to the list of known hosts.
ctf-player@saturn.picoctf.net's password: 
Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 6.5.0-1023-aws x86_64)

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

Special$ ls
Is 
sh: 1: Is: not found
Special$ -h 
Oh 
sh: 1: Oh: not found
Special$ I
I 
sh: 1: I: not found
Special$ IS
IS 
sh: 1: IS: not found
Special$ Is
Is 
sh: 1: Is: not found
Special$ sh
Why go back to an inferior shell?
Special$ Help
Help 
sh: 1: Help: not found
Special$ dir
Dir 
sh: 1: Dir: not found
Special$ DIR
DIR 
sh: 1: DIR: not found
Special$ ls
Is 
sh: 1: Is: not found
Special$ cat
Cat 
sh: 1: Cat: not found
Special$ --help
Help 
sh: 1: Help: not found
Special$ ls -help
Is help 
sh: 1: Is: not found
Special$ /info
Absolutely not paths like that, please!
Special$ cd
Ad 
sh: 1: Ad: not found
Special$ c
I 
sh: 1: I: not found
Special$ cd
Ad 
sh: 1: Ad: not found
Special$ cdcd
Did 
sh: 1: Did: not found
Special$ sdsd
Did 
sh: 1: Did: not found
Special$ asas
Ass 
sh: 1: Ass: not found
Special$ ess
Ess 
sh: 1: Ess: not found
Special$ eses
Eses 
sh: 1: Eses: not found
Special$ erer
Ever 
sh: 1: Ever: not found
Special$ rtrt
Try 
sh: 1: Try: not found
Special$ list
List 
sh: 1: List: not found
Special$ $pwd
Pod 
sh: 1: Pod: not found
Special$ whoami
Whom 
sh: 1: Whom: not found
Special$ echo $foo
Echo foo 
sh: 1: Echo: not found
Special$ set foo bar
Set foo bar 
sh: 1: Set: not found
Special$ ((ls))
((ls)) 
blargh
Special$ (ls)   
Also 
sh: 1: Also: not found
Special$ ((ls))
((ls)) 
blargh
Special$ ((ls -la))
Pals -la)) 
sh: 1: Syntax error: ")" unexpected
Special$ ((cat)) < blargh/flag.txt
((cat)) < blargh/flag.txt 
picoCTF{5p311ch3ck_15_7h3_w0r57_b741d1b1}Special$ 
Traceback (most recent call last):
  File "/usr/local/Special.py", line 19, in <module>
    elif cmd[0] == '/':
IndexError: string index out of range
Connection to saturn.picoctf.net closed.
```