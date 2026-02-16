# fixme2.py

## Descripción
Fix the syntax error in the Python script to print the flag.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/5/fixme2.py
VictorCervantes-picoctf@webshell:~$ ls
fixme2.py
VictorCervantes-picoctf@webshell:~$ python fixme2.py 
  File "/home/VictorCervantes-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
VictorCervantes-picoctf@webshell:~$ nano fixme2.py 
VictorCervantes-picoctf@webshell:~$ python fixme2.py 
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
## Notas adicionales
- 

## Referencias
- 