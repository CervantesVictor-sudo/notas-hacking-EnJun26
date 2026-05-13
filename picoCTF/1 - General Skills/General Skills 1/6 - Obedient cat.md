# Obedient cat

## Descripción
This file has a flag in plain sight (aka "in-the-clear").
## Solución
```
VictorCervantes-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/4acf636990e4540d6fc36684b1256e625c0617d7cb01727e12e3f9606d89fe45/flag
--2026-02-09 14:33:11--  https://challenge-files.picoctf.net/c_wily_courier/4acf636990e4540d6fc36684b1256e625c0617d7cb01727e12e3f9606d89fe45/flag
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.18, 3.160.5.64, 3.160.5.95, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.18|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag               100%[==============>]      34  --.-KB/s    in 0s      

2026-02-09 14:33:11 (1.46 MB/s) - 'flag' saved [34/34]

VictorCervantes-picoctf@webshell:~$ cat flag
picoCTF{s4n1ty_v3r1f13d_9b8fa0bc}
VictorCervantes-picoctf@webshell:~$ 
```
picoCTF{s4n1ty_v3r1f13d_9b8fa0bc}
## Notas adicionales
- 
## Referencias
- 