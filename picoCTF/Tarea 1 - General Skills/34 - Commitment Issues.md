## Commitment Issues

## Descripción
I accidentally wrote the flag down. Good thing I deleted it!
You download the challenge files here: challenge.zip

## Solución

```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/76/challenge.zip
VictorCervantes-picoctf@webshell:~$ ls
README.txt  challenge.zip
VictorCervantes-picoctf@webshell:~$ unzip challenge.zip 
VictorCervantes-picoctf@webshell:~$ ls
README.txt  challenge.zip  drop-in
VictorCervantes-picoctf@webshell:~$ cd drop-in/
VictorCervantes-picoctf@webshell:~/drop-in$ ls
message.txt
VictorCervantes-picoctf@webshell:~/drop-in$ cat message.txt 
TOP SECRET
VictorCervantes-picoctf@webshell:~/drop-in$ ls -la
total 12
drwxr-xr-x 3 VictorCervantes-picoctf VictorCervantes-picoctf   49 Mar  9  2024 .
drwxr-xr-x 5 VictorCervantes-picoctf VictorCervantes-picoctf 4096 Feb 21 04:42 ..
drwxr-xr-x 8 VictorCervantes-picoctf VictorCervantes-picoctf 4096 Mar  9  2024 .git
-rw-r--r-- 1 VictorCervantes-picoctf VictorCervantes-picoctf   11 Feb 21 04:42 message.txt
```
Al ver que la carpeta estaba conectada a un git, usé comandos para ver el historial de cambios que se hicieron y asi regresar el repositorio a un anterior commit usando el ID del commit.
```
VictorCervantes-picoctf@webshell:~/drop-in$ git log
VictorCervantes-picoctf@webshell:~/drop-in$ git checkout e720dc26a1a55405fbdf4d338d465335c439fb3e
Note: switching to 'e720dc26a1a55405fbdf4d338d465335c439fb3e'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at e720dc2 create flag
VictorCervantes-picoctf@webshell:~/drop-in$ ls
message.txt
VictorCervantes-picoctf@webshell:~/drop-in$ cat message.txt 
picoCTF{s@n1t1z3_7246792d}

```
picoCTF{s@n1t1z3_7246792d}
## Notas adicionales
- 'git log' para ver el historial de commits que se hicieron y ver el ID de los mismos.
- 'git checkout {id}' en donde es necesario el id del commit al que quieras regresar ese repositorio.

## Referencias
- https://primer.picoctf.org/#_review_of_git