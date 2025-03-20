
#### Description

This website can be rendered only by **picobrowser**, go and catch the flag! `https://jupiter.challenges.picoctf.org/problem/28921/` ([link](https://jupiter.challenges.picoctf.org/problem/28921/)) or http://jupiter.challenges.picoctf.org:28921

Solucion: 

algo parecido a cambiar las cookies, pero en este caso solo es cambiar un header, como chrome no sive para este caso use la shell de picoctf...

Usando un comando curioso:  curl -s https://jupiter.challenges.picoctf.org/problem/28921/flag -H "User-Agent:picobrowser" | grep picoCTF

lo que hacemos es que del todo el codigo, solo agarre la parte del picoctf

