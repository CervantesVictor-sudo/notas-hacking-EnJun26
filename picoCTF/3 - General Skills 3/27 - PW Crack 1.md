# PW Crack 1

## Descripción
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/11/level1.py
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
VictorCervantes-picoctf@webshell:~$ ls
level1.flag.txt.enc  level1.py
VictorCervantes-picoctf@webshell:~$ nano level1.py
VictorCervantes-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_fa343060}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{545h_r1ng1ng_fa343060}
## Notas adicionales
- Modificamos el archivo .py para saber la contraseña correcta al estar escrita de manera explícito en el código.

## Referencias
- 