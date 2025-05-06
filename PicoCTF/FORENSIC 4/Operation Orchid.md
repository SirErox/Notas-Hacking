descripcion:
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/214/disk.flag.img.gz)

solucion:
use autopsy para mejor trabajo, e igual, me puse a urgar en el directorio de root y encontre lo necesario...

el archivo encodificado, junto con el comando usado para la codificacion...

asi que solo es poner el comando mismo que usaron, pero ahora con unos cambios leves:

	openssl aes256 -d -salt -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567

y en ese archivo tendremos la bandera...
picoCTF{h4un71ng_p457_1d02081e}