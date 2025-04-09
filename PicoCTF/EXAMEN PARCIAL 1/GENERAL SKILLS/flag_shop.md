descripcion:
There's a flag shop selling stuff, can you buy a flag? [Source](https://jupiter.challenges.picoctf.org/static/64e724ad327f83ad833d9c6baa072b1f/store.c). Connect with `nc jupiter.challenges.picoctf.org 4906`.

solucion:
los enteros con signo tienen un rango por asi decirlo, y en una parte del codigo se mueve ese rango sin querer...

cuando nos conectamos al servidor vemos que podemos comprar unas banderas knockoff, pero son baratas, y es donde vamos a alterar el codigo, le decimos que queremos 3000000, para que altere el dinero total que tenemos

despues vamos a comprar la bandera real y ya lo tenemos.
picoCTF{m0n3y_bag5_9c5fac9b}