# Time machine

## Descripción
What was I last working on? I remember writing a note to help me remember...
You download the challenge files here: challenge.zip

## Solución

```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/66/challenge.zip
VictorCervantes-picoctf@webshell:~$ unzip challenge.zip
VictorCervantes-picoctf@webshell:~$ ls
challenge.zip  drop-in
VictorCervantes-picoctf@webshell:~$ cd drop-in/
VictorCervantes-picoctf@webshell:~/drop-in$ ls
message.txt
VictorCervantes-picoctf@webshell:~/drop-in$ cat message.txt 
This is what I was working on, but I'd need to look at my commit history to know why...
VictorCervantes-picoctf@webshell:~/drop-in$ cd .git/
VictorCervantes-picoctf@webshell:~/drop-in/.git$ ls
COMMIT_EDITMSG  branches  description  index  logs     refs
HEAD            config    hooks        info   objects
VictorCervantes-picoctf@webshell:~/drop-in/.git$ cd logs/
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs$ ls
HEAD  refs
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs$ cd refs/
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs/refs$ ls
heads
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs/refs$ cd heads/
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs/refs/heads$ ls
master
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs/refs/heads$ cat master 
0000000000000000000000000000000000000000 3339c144a0c78dc2fbd3403d2fb37d3830be5d94 picoCTF <ops@picoctf.com> 1710018622 +0000      commit (initial): picoCTF{t1m3m@ch1n3_d3161c0f}
VictorCervantes-picoctf@webshell:~/drop-in/.git/logs/refs/heads$ 

```
picoCTF{t1m3m@ch1n3_d3161c0f}
## Notas adicionales
- 

## Referencias
- 