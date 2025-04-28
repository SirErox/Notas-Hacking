descripcion:

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

solucion:

en este reto tenemos paquetes igual que shark on a wire, pero esta vez esta mas oculta la bandera y no tan a la vista... ahora esta oculta en unos numeros, cuando vemos los paquetes UDP, vemos que dice START y al final END,  unos numeros que van 5000 mas o menos, se ven curiosos, si les restamos los 5000 y convertimos a caracter ascii vemos que son letras de la bandera como tal...

pero no queremos capturar letra por letra, asi que hacemos un script para sacar esos caracteres... dicho script lo saque del video:
https://www.youtube.com/watch?v=WcMl1SvQ6hI&ab_channel=hackadvisermx
script: 

	from scapy.all import *
	packets=rdpcap('capture.pcap')
	flag=""

	for p in packets:
    if UDP in p and p[UDP].dport==22:
        if p[UDP].sport > 5000:
            flag +=chr(p[UDP].sport-5000)

	print(flag)

picoCTF{p1LLf3r3d_data_v1a_st3g0}