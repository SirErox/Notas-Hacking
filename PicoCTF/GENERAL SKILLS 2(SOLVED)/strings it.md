Reto: ### strings it

Descripcion:
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it? 

hints: https://linux.die.net/man/1/strings

Solucion:
	Para este reto primero descargue el archivo y al darle un cat me dio mucha informacion... asi que use la pista, y me dice que ponga un strings usando el piping...
```
cat strings | strings
```
pero al hacerlo salen muchas cadenas de texto que abruman... a lo cual se me ocurrio ponerle otro comando que ya conocemos grep...

```
cat strings | strings | grep "pico"
```
y directamente nos suelta la bandera...

picoCTF{5tRIng5_1T_7f766a23}