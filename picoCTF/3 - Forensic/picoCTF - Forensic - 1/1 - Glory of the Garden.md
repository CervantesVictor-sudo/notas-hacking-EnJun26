# Glory of the Garden

## Descripción
This file contains more than it seems.
Get the flag from [garden.jpg](https://challenge-files.picoctf.net/c_fickle_tempest/19722024edeecca10f263776ab05c8b1235b136dcf25aa6e976d3860513ffcd5/garden.jpg).

## Solución

```
VictorCervantes-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_tempest/19722024edeecca10f263776ab05c8b1235b136dcf25aa6e976d3860513ffcd5/garden.jpg
--2026-03-09 14:09:44--  https://challenge-files.picoctf.net/c_fickle_tempest/19722024edeecca10f263776ab05c8b1235b136dcf25aa6e976d3860513ffcd5/garden.jpg
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.64, 3.160.5.18, 3.160.5.95, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.64|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 2295191 (2.2M) [application/octet-stream]
Saving to: 'garden.jpg'

garden.jpg         100%[==============>]   2.19M  1.83MB/s    in 1.2s    

2026-03-09 14:09:45 (1.83 MB/s) - 'garden.jpg' saved [2295191/2295191]

VictorCervantes-picoctf@webshell:~$ strings garden.jpg | grep pico
Here is a flag: picoCTF{more_than_m33ts_the_3y37fde8891}
VictorCervantes-picoctf@webshell:~$ 


```

picoCTF{more_than_m33ts_the_3y37fde8891}
## Notas adicionales
- 

## Referencias
- 