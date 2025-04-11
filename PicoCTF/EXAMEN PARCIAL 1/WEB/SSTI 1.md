DESCRIPCION:
I made a cool website where you can announce whatever you want! Try it out!

SOLUCION:
el reto nos incluye algo nuevo, el server-side template inyection, que es usar una vulnerabilidad, como poner doble {{ }} para colar codigo en el sistema...

https://www.onsecurity.io/blog/server-side-template-injection-with-jinja2/ en este sitio encontre algunos comandos como:

	{{request.application.__globals__.__builtins__.__import__('os').popen('id').read()}}
solo remplaze el ID por un ls por ejemplo...

y me dice que hay unos archivos, asi como flag... 
asi que solo le puse un cat flag y me dio la bandera
picoCTF{s4rv3r_s1d3_t3mp14t3_1nj3ct10n5_4r3_c001_73c99823}