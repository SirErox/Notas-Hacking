#### Description

Can you read files in the root file?

Solucion:
	Para este reto si tuve que buscar informacion... asi que encontre este writeup...
https://medium.com/@petemuiruri/permissions-writeup-picoctf-2023-be95c95f80a5

Nos dice que al conectarnos al servidor debemos checar que permisos tenemos, y para eso esta el comando sudo -l

Y nos dice que para poder entrar como root debemos poner un comando especial "sudo vi test" junto con :!/bin/bash, y asi abriremos un espacio root, nos movemos al directorio raiz, y veremos un archivo que dice .flag.txt, le damos un cat y tenemos la respuesta

picoCTF{uS1ng_v1m_3dit0r_3dd6dcf4}