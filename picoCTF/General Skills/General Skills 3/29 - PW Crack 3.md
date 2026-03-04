# PW Crack 3

## Descripción
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/16/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/16/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/16/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/16/level3.py
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/16/level3.flag.txt.enc
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/16/level3.hash.bin
VictorCervantes-picoctf@webshell:~$ nano level3.py
VictorCervantes-picoctf@webshell:~$ python level3.py 
Please enter correct password for flag: 865e
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_2b072a90}
VictorCervantes-picoctf@webshell:~$ 

```

Flag: picoCTF{m45h_fl1ng1ng_2b072a90}
## Notas adicionales
- Dentro del archivo .py, vienen las cadenas que podían ser la contraseña, intenté al azar con todas hasta que encontré la correcta.

## Referencias
- 