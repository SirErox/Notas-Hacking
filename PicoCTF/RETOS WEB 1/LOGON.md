#### Description

The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/13594/` ([link](https://jupiter.challenges.picoctf.org/problem/13594/)) or http://jupiter.challenges.picoctf.org:13594

Solucion:
Para este reto se ocupa una herramienta COOKIE EDITOR decente! porque si no vas a batallar demasiado...

Segun la informacion, en las cookies se guarda mucha informacion que sabiendola usar es peligrosa, por ende, hay un parametro que se guarda en esas cookies una vez que queremos loguearnos...

admin=False, con lo cual solo tenemos que cambiar ese valor por True y podremos ver la bandera:

picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}
