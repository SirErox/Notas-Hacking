descripcion:
	
	A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/586d0206891cc683bae1160ad6b0e05d7e10e7b2df122c0441ab06581038dd32/myNetworkTraffic.pcap) and try to get the flag.

solucion:

	al abrir wireshark, vemos que son pocos paquetes y son puros tcp, en las pistas del reto nos decia de aplicar un filtro y que el tiempo es escencial, asi que primero aplico un filtro donde los paquetes tengan entre 4 y 12 bytes de payload, y que me los organize por tiempo.... conforme vi los paquetes, las cadenas puestas estaban codificadas en base64...
	
cGljb0NURg==
ezF0X3c0cw==
bnRfdGg0dA==
XzM0c3lfdA==
YmhfNHJfMg==
ZTFmZjA2Mw==
fQ==


	picoCTF{1t_w4snt_th4t_34sy_tbh_4r_2e1ff063}