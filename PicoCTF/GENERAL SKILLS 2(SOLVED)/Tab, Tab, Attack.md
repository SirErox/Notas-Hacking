Reto: ### Tab, Tab, Attack

Descripcion: Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames: [Addadshashanammu.zip](https://mercury.picoctf.net/static/9689f2b453ad5daeb73ca7534e4d1521/Addadshashanammu.zip)

Hints: After `unzip`ing, this problem can be solved with 11 button-presses...(mostly Tab)..

Solucion:

Al descargar el archivo primero use `unzip -l xxx.zip` para ver que contenia y vi que en el directorio mas largo habia un archivo...

Asi que use un pipe con grep para ver si estaba la bandera que ocupaba y si, el comando no me podia regresar la bandera pero si me confirmaba que existia...

Sin pensar use el comando strings y vi que salio la bandera entre tanto texto, pero para evitar mas problemas se puede usar el comando completo
```
cat Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet | strings | grep "pico"
```
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_2bcfb2ab}
