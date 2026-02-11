# Strings it

## Descripción
Can you find the flag in [file](https://challenge-files.picoctf.net/c_fickle_tempest/285538e2710605958a055500d6573657fcafea6308545cecfabb34462199cfd5/strings) without running it?

## Solución
```
VictorCervantes-picoctf@webshell:~$ file strings
strings: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=f4f3c992bb3f870f5b303cb391db44c8f665d4a9, for GNU/Linux 3.2.0, not stripped
VictorCervantes-picoctf@webshell:~$ ls -la strings
-rw-rw-r-- 1 VictorCervantes-picoctf VictorCervantes-picoctf 784424 Nov 14 19:58 strings
VictorCervantes-picoctf@webshell:~$ chmod -x strings
VictorCervantes-picoctf@webshell:~$ ls -la strings
-rw-rw-r-- 1 VictorCervantes-picoctf VictorCervantes-picoctf 784424 Nov 14 19:58 strings
VictorCervantes-picoctf@webshell:~$ ./ strings
-bash: ./: Is a directory
VictorCervantes-picoctf@webshell:~$ strings strings | grep pico
picoCTF{5tRIng5_1T_1067EC4c}

```
## Notas adicionales
- 

## Referencias
- 