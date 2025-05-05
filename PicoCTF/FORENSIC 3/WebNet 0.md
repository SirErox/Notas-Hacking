Descripcion:
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

solucion:
cargamos lo necesario en la maquina virtual, primero vemos que son captura de paquetes de red, asi que ocupamos wireshark...

al ver la secuencia de paquetes, vemos que hay algunos "TLS"

	TLS:La Seguridad de la Capa de Transporte (TLS) es un protocolo criptográfico diseñado para proporcionar seguridad en las comunicaciones a través de una red informática, como Internet. El protocolo se usa ampliamente en aplicaciones como el correo electrónico, la mensajería instantánea y la voz sobre IP, pero su uso para proteger HTTPS sigue siendo el más visible.

y casualmente nos dieron una llave para desencriptar esos paquetes... asi que hay que pasarsela al wireshark, en preferencias y sobre protocolos, para despues ir hasta TLS y en rsa... para cargar ese archivo...

ya una vez que esta cargada esa llave, se "desencriptan" esos paquetes, y con un find podemos encontrar la llave correcta...


picoCTF{nongshim.shrimp.crackers}