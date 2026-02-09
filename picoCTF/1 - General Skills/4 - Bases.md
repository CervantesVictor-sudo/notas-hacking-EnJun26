# Bases

## Descripción
What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.
## Solución 1 - terminal linux
```
VictorCervantes-picoctf@webshell:~$ echo 'bDNhcm5fdGgzX3IwcDM1' | base64 -d
l3arn_th3_r0p35VictorCervantes-picoctf@webshell:~$ 
```
picoCTF{l3arn_th3_r0p35}
## Solucion 2 - python
```
VictorCervantes-picoctf@webshell:~$ python
Python 3.10.12 (main, Feb  4 2025, 14:57:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import base64
>>> base64.b64decode('bDNhcm5fdGgzX3IwcDM1')
b'l3arn_th3_r0p35'
>>> 
```
## Solucion 3
- https://gchq.github.io/CyberChef/#recipe=To_Base64('A-Za-z0-9%2B/%3D')&input=YkROaGNtNWZkR2d6WDNJd2NETTE
## Notas adicionales
- Usamos la pagina de cyberchef para resolver el reto
- Se uso la terminal de Pico para resolver el reto mediante linux
- Se uso la terminal de Pico para resolver el reto mediante linux
## Referencias
- https://gchq.github.io/CyberChef/