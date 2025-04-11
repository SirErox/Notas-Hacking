descripcion:
	Welcome to the challenge! In this challenge, you will explore a web application and find an endpoint that exposes a file containing a hidden flag.The application is a simple blog website where you can read articles about various topics, including an article about API Documentation. Your goal is to explore the application and find the endpoint that generates files holding the server’s memory, where a secret flag is hidden.

solucion:
al cargar la pagina vemos que estsa mas o menos diseñada, pero hay unos hastags que no se ven interensantes, al dar click en api documentation nos vamos directo a la api y no a donde deberia...

estando dentro vemos un comando que dice headdump o algo parecido hasta el final de la pagina, nos dara un archivo a descargar, para este archivo lo puse en una maquina con linux, aplicamos un cat y la tecnica de pipeing con un grep... y lo primero es la bandera...


picoCTF{Pat!3nt_15_Th3_K3y_ad7ea5ae}