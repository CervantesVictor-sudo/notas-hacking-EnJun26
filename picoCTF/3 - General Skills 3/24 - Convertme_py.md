# Convertme_py

## Descripción
Run the Python script and convert the given number from decimal to binary to get the flag.

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/23/convertme.py
VictorCervantes-picoctf@webshell:~$ ls  
convertme.py
VictorCervantes-picoctf@webshell:~$ python convertme.py 
If 31 is in decimal base, what is it in binary base?
Answer: 11111
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_9c3b7d4d}
VictorCervantes-picoctf@webshell:~$ 

```
Se utilizó CyberChef para hacer la conversion de base decimal a binario: https://gchq.github.io/CyberChef/#recipe=To_Base(2)&input=MzE

picoCTF{4ll_y0ur_b4535_9c3b7d4d}
## Notas adicionales
- En CyberChef, utilizamos el 'to base' con radix en 2, para obtener la respuesta ingresando solo el numero solicitado.

## Referencias
- 