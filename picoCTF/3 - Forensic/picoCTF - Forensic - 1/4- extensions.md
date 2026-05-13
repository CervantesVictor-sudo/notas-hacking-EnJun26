# extensions

## Descripción
This is a really weird text file. Can you find the flag?
Get the flag from [TXT](https://challenge-files.picoctf.net/c_fickle_tempest/31fe772e6a4c71e867af0b2a93818e06d8f8ebf8af2a9615495d00356ff576da/flag.txt).

## Solución

```
VictorCervantes-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_tempest/31fe772e6a4c71e867af0b2a93818e06d8f8ebf8af2a9615495d00356ff576da/flag.txt
VictorCervantes-picoctf@webshell:~$ xxd -l 20 flag.png 
00000000: 8950 4e47 0d0a 1a0a 0000 000d 4948 4452  .PNG........IHDR
00000010: 0000 06a1                                ....
VictorCervantes-picoctf@webshell:~$ mv flag.txt flag.png 
VictorCervantes-picoctf@webshell:~$ open flag.png 

```

picoCTF{now_you_know_about_extensions}

## Notas adicionales
- 

## Referencias
- 