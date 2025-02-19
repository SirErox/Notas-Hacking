reto PW CRACK 2

#### Description

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/14/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) in the same directory too.

Solucion:

	Al hacer un cat al archivo vi que de nuevo hace una comparacion directa, pero esta ves usa una funcion para esconder esos caracteres que ocupamos...
```
def level_2_pw_check():
    user_pw = input("Please enter correct password for flag: ")
    if( user_pw == chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39) ):
        print("Welcome back... your flag, user:")
        decryption = str_xor(flag_enc.decode(), user_pw)
        print(decryption)
        return
    print("That password is incorrect")
```

Asi que abri el interprete de python en la consola y puse esa serie de chrs, dandome 4ec9, asi que le di esos caracteres al programa y me dio la bandera

	picoCTF{tr45h_51ng1ng_9701e681}
