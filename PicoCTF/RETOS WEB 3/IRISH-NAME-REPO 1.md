descripcion: 
There is a website running at `https://jupiter.challenges.picoctf.org/problem/33850/` ([link](https://jupiter.challenges.picoctf.org/problem/33850/)) or http://jupiter.challenges.picoctf.org:33850. Do you think you can log us in? Try to see if you can login!

solucion:

para este reto nos piden conocer de sql inyection, que basicamente aprovecha vulnerabilidades del mismo lenguaje...

por ejemplo, si yo comparo una cadena"password" con alguna en la base, se puede brincar ese chequeo y hacerle creer al sistema que tenemos los datos correctos

	en este caso pondremos el tipico usuario admin y en password 'OR 1==1; 
en esa linea de codigo hacemos que cualquier contraseña que nosotros ingresemos no sea verificada y el codigo crea que si es valida...

picoCTF{s0m3_SQL_f8adf3fb}