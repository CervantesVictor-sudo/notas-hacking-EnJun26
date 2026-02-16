# fixme1.py

## Descripción
Fix the syntax error in this Python script to print the flag.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/27/fixme1.py
VictorCervantes-picoctf@webshell:~$ python fixme1.py 
  File "/home/VictorCervantes-picoctf/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
VictorCervantes-picoctf@webshell:~$ nano fixme1.py 
VictorCervantes-picoctf@webshell:~$ python fixme1.py 
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_182342f7}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{1nd3nt1ty_cr1515_182342f7}
## Notas adicionales
- 

## Referencias
- 