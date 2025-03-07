Descripcion:
Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag!Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz).

Solucion:
Para este reto tuve que instalar rust en linux
https://doc.rust-lang.org/book/ch01-01-installation.html en esta pagina se encuentra todo para la instalacion...

ya una vez instalado, no intentes ir directo a buscar el archivo main.rs porque solo te toparas con los errores... queremos la bandera

Primero una ves que descomprimes el archivo y entras al directorio fixme1 aplica un comando "cargo build" esto para ver que proyecto es y poder resolverlo...

Incluso cuando lo esta construyendo te aparecen los errores y que archivo tenemos que corregir...

Cuando entras a ver el main, te hace preguntas clarisimas... y algunas con trampas


https://doc.rust-lang.org/cargo/getting-started/first-steps.html
https://doc.rust-lang.org/std/macro.println.html 

me la pase buscando en estas 2 paginas, la sintaxis del lenguaje de rust, un poco complicado de entender pero esta bien...

Ya una vez que resuelvas los errores, puedes comprobar de nuevo con el comando de cargo build, si todo esta bien, vas a ejecutar el archivo que esta dentro de la carpeta target...

y te soltara la bandera..

