# Binhexa

## Descripción
How well can you perfom basic binary operations?
Start searching for the flag here `nc titan.picoctf.net 61508`

## Solución
```
VictorCervantes-picoctf@webshell:~$ nc titan.picoctf.net 61508

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10100110
Binary Number 2: 01100000


Question 1/6:
Operation 1: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00100000
Correct!

Question 2/6:
Operation 2: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111001000000           
Correct!

Question 3/6:
Operation 3: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11100110
Correct!

Question 4/6:
Operation 4: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 100000110
Correct!

Question 5/6:
Operation 5: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 101001100
Correct!

Question 6/6:
Operation 6: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 00110000
Correct!

Enter the results of the last operation in hexadecimal: 0x30

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d9a7ddd2}

VictorCervantes-picoctf@webshell:~$ 

```

picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d9a7ddd2}
## Notas adicionales
- 

## Referencias
- 