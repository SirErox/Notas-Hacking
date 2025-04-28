descripcion:
We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.

solucion:
en este reto te recomiendo primero instalar pngchecker:

	sudo apt install pngchecker

ya que el archivo a tratar se trata de un png, que la cabecera esta dañada, casi todos los archivos tienen ese header o cabecera, que le dice a la computadora que contiene y de que trata, y adentro de ese header, debe haber ciertos parametros para que se considere correcto el archivo, png checker nos ayudara con eso...

si el chunk de tal informacion no coincide, hay que hacer que coincidan las letras... tambien hay una mejor version explicada en :

https://www.youtube.com/watch?v=7zY4VkiWbBI&ab_channel=hackadvisermx

picoCTF{c0rrupt10n_1847995}