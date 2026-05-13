# Big zip

## Descripción
Unzip this archive and find the flag.
- **Download zip file**

## Solución
```
VictorCervantes-picoctf@webshell:~$ ls
README.txt  big-zip-files  big-zip-files.zip
VictorCervantes-picoctf@webshell:~$ cd big-zip-files/
VictorCervantes-picoctf@webshell:~/big-zip-files$ grep -r pico
folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}
VictorCervantes-picoctf@webshell:~/big-zip-files$ 

```
picoCTF{gr3p_15_m4g1c_ef8790dc}
## Notas adicionales
- El comando 'grep -r pico' busca de manera recursiva la palabra "pico" en todos los archivos

## Referencias
- 