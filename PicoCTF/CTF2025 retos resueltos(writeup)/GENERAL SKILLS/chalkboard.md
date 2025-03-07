#### Description

Bart's up to his old tricks on the chalkboard again. This time, he's filled a large file with his favorite phrase. I wonder why!Download Chalkboard [here](https://challenge-files.picoctf.net/c_verbal_sleep/905b0f69cffd3be24c8a80d056fa05667d5e706a5740a701ec60f7bd36660119/chalkboardgag.txt).

Solucion:
Descargando el archivo, veo que es repetitivo... la misma frase, le aplique el "grep "pico" " pero no solto nada, con lo cual me dice que esta fragmentada, despues de buscar las opciones de grep, hay una que podria servirme...

La frase es repetitiva, y si la traducimos deberia decir que "no sere escurridizo" o algo asi

ocupamos quitar esa frase, y dejar solo los caracteres que no pertenezcan a la frase... asi que le decimos que a la salida del comando grep quite tolo lo que coincida con esa frase... y nos dara una lista de caracteres en vertical de la bandera...

pero ocupamos ponerla en horizontal, asi que investigando en internet, el comando tr puede ser util...

Asi que usamos pipeing.. 

tr -d '/n' indica que vamos a quitar los saltos de linea y juntaremos los caracteres en una sola linea

grep -o '[^I WILL NOT BE SNEAKY]' chalkboardgag.txt | tr -d '/n'


