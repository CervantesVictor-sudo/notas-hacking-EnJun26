# Tab, Tab, Attack

## Descripción
Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames.

## Solución
Primero, descargamos y descomprimimos la carpeta zip:
```
VictorCervantes-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/47c062933bddfd5b44f49ffc357a9a0a9628b94694f93de98724da39504c0a93/Addadshashanammu.zip
--2026-02-11 14:43:25--  https://challenge-files.picoctf.net/c_wily_courier/47c062933bddfd5b44f49ffc357a9a0a9628b94694f93de98724da39504c0a93/Addadshashanammu.zip
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.40, 3.160.5.95, 3.160.5.64, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.40|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 5166 (5.0K) [application/octet-stream]
Saving to: 'Addadshashanammu.zip'

Addadshashanammu.z 100%[==============>]   5.04K  --.-KB/s    in 0s      

2026-02-11 14:43:25 (45.3 MB/s) - 'Addadshashanammu.zip' saved [5166/5166]

VictorCervantes-picoctf@webshell:~$ unzip Addadshashanammu.zip 

```
Despues, hacemos tab hasta encontrar el ultimo archivo y lo ejecutamos:
```
VictorCervantes-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt
VictorCervantes-picoctf@webshell:~$ cd Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/
VictorCervantes-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmi
milkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ls
fang-of-haynekhtnamet  fang-of-haynekhtnamet.c
VictorCervantes-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmi
milkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ file fang-of-haynekhtnamet
fang-of-haynekhtnamet: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=4fdc1b4e898a0612ce5aa28e5012209f20bfc0ca, for GNU/Linux 3.2.0, not stripped
VictorCervantes-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmi
milkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ./fang-of-haynekhtnamet 
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_fc588427}
VictorCervantes-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmi
milkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ cd
VictorCervantes-picoctf@webshell:~$

```
picoCTF{l3v3l_up!_t4k3_4_r35t!_fc588427}
## Notas adicionales
- 

## Referencias
- 