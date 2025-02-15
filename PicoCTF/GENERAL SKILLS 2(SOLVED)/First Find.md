Reto: ### FIRST FIND

Descripcion:
Unzip this archive and find the file named 'uber-secret.txt'

solucion:
Ya la descripcion nos da una idea, de que es hacer unzip y usar algo mas...

Primero use unzip para sacar todo, luego hice un unzip -l files.zip, y vi el archivo... bastante escondido

Asi que ahora solo me quedaba sacar la bandera de ese archivo, use la tecnica de pipes

unzip files.zip | grep -r "pico"
```
┌──(kali㉿kali)-[~/files]
└─$ unzip files.zip | grep -r "pico"
adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt:picoCTF{f1nd_15_f457_ab443fd1}

```