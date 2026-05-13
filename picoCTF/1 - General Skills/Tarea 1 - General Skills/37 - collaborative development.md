# Collaborative development

## Descripción
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?
You download the challenge files here: challenge.zip

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/71/challenge.zip
VictorCervantes-picoctf@webshell:~$ unzip challenge.zip
VictorCervantes-picoctf@webshell:~$ ls
challenge.zip  drop-in
VictorCervantes-picoctf@webshell:~$ cd drop-in/
VictorCervantes-picoctf@webshell:~/drop-in$ git branch -a
VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
VictorCervantes-picoctf@webshell:~/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
picoCTF{t3@mw0rk_VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.git checkout feature/part-2
Switched to branch 'feature/part-2'
VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
m@k3s_th3_dr3@m_VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.pgit checkout feature/part-3
Switched to branch 'feature/part-3'
VictorCervantes-picoctf@webshell:~/drop-in$ python3 flag.py 
Printing the flag...
w0rk_4c24302f}
VictorCervantes-picoctf@webshell:~/drop-in$ 

```

picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_4c24302f}

## Notas adicionales
- Al usar 'git branch -a' me aparecieron todas las ramas que tiene el repositorio, marcando en verde en la que me encuentro actualmente.
- Al usar 'git checkout {branch}' me sirvió para moverme entre ramas escribiendo el nombre que me aparecían con el comando 'git branch -a'.
- Al estar en cada una de las ramas, utilice el comando 'nano' para abrir y editar el archivo python que tenia cada rama, así pude darme cuenta que era lo que imprimía y solo junté cada impresión de cada rama para conseguir la flag.

## Referencias
- 