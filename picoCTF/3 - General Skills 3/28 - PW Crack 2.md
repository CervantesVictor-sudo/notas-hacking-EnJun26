# PW Crack 2

## Descripción
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/14/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) in the same directory too.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/14/level2.py
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/14/level2.flag.txt.enc
VictorCervantes-picoctf@webshell:~$ ls
level2.flag.txt.enc  level2.py
VictorCervantes-picoctf@webshell:~$ nano level2.py
VictorCervantes-picoctf@webshell:~$ python level2.py 
4ec9
Please enter correct password for flag: 4ec9
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_9701e681}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{tr45h_51ng1ng_9701e681}
## Notas adicionales
- Modificamos el archivo .py para poder saber los caracteres por medio de la linea:
  'print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))', ya que esos son comandos que puede leer python sin problema y darnos la respuesta correcta.

## Referencias
- 