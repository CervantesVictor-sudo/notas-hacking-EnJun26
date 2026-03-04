# Plumbing

## Descripción
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag?
'Additional details will be available after launching your challenge instance.'

Connect to fickle-tempest.picoctf.net 65298.
## Solución 1
```
VictorCervantes-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 65298 | grep pico
picoCTF{digital_plumb3r_0BAc587E}

```
picoCTF{digital_plumb3r_0BAc587E}

# solucion 2
```
VictorCervantes-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 49621 > salida

VictorCervantes-picoctf@webshell:~$ cat salida | grep pico
picoCTF{digital_plumb3r_0BAc587E}

```
## Notas adicionales
- Para este caso, al no utilizar el 'grep' en la terminal nos arroja de salida mucha informacion y repetitiva y no podemos encontrar la respuesta, por eso al filtrar con grep ahora si obtenemos la respuesta.
- '>', redirige la salida de un comando a un archivo.
## Referencias
- 