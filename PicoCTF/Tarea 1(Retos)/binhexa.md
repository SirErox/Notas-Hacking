How well can you perfom basic binary operations?

Additional details will be available after launching your challenge instance.

Solucion:
En este reto solo nos piden hacer operaciones con numeros en binario... asi que me puse a buscar en internet diferentes paginas que me ayudasen a hacer esas operaciones..
```
nc titan.picoctf.net 53925             

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 11111111
Binary Number 2: 00110010


Question 1/6:
Operation 1: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 100110001
Incorrect. Try again
Enter the binary result: 00110010
Correct!

Question 2/6:
Operation 2: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111111
Correct!

Question 3/6:
Operation 3: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 00011001.

Incorrect input. Provide the right input
Enter the binary result: 00011001
Correct!

Question 4/6:
Operation 4: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 0100110001
Correct!

Question 5/6:
Operation 5: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 11111111
Incorrect. Try again
Enter the binary result: 11111111
Incorrect. Try again
Enter the binary result: 000111111110
Correct!

Question 6/6:
Operation 6: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 011000111001110
Correct!

Enter the results of the last operation in hexadecimal: 634e
Incorrect answer!

Enter the results of the last operation in hexadecimal: 63 4e

Incorrect input. Provide the right input!

Enter the results of the last operation in hexadecimal: 31CE

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_675602ae}
```