descripcion:
Can you win in a convincing manner against this chess bot? He won't go easy on you!You can find the challenge [here](http://verbal-sleep.picoctf.net:61344/).


solucion:

para este reto vi el siguiente video:

https://www.youtube.com/watch?v=xqopwb8Iv90&ab_channel=hackadvisermx

al parecer es un pescado jugandole al ajedrez, pero usaremos la consola de chrome, hay un comando que se llama sendMessage() y pondremos el valor de una variable que indica si el va perdiendo o ganando...

sendMessage("eval -100000") este comando le hace creer al pescado que va perdiendo la partida, en caso dado de que no funcione, solo es aumentar ese valor y esperar que suelte la bandera, o tambien puedes intentar vencerlo justamente...

picoCTF{c1i3nt_s1d3_w3b_s0ck3t5_a2a9bbe9}