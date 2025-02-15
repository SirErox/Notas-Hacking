Reto: ### Big Zip

Descripcion:
Unzip this archive and find the flag.

hints: Can grep be instructed to look at every file in a directory and its subdirectories?

Solucion: Primero tuve que investigar como abrir un .zip en consola de comandos...

Despues quise intentar abrirlo y me di cuenta que esta diseñado para soltar muchos archivos sin fin, asi que tome encuenta el grip y la tecnica de pipeing...

Solo que antes investigue mas del comando grep, resulta que tiene una opcion "-r" que hace que sea recursiva, ayudandonos en directorios grandes...

Asi que el comando que use fue "unzip big-zip-file.zip | grep -r"pico"
```
README.txt:Welcome to the picoCTF webshell!
README.txt:picoCTF challenges.
README.txt:other@picoctf.org and we will consider adding it.
README.txt:  Extensive brute-forcing is not necessary to solve picoCTF challenges.
README.txt:- If you change your username through the picoCTF website, you will
bigzip/big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}
```
