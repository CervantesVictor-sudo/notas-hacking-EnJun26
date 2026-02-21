# Blame game

## Descripción
Someone's commits seems to be preventing the program from working. 
Who is it?
You download the challenge files here: challenge.zip

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_titan/158/challenge.zip
VictorCervantes-picoctf@webshell:~$ unzip challenge.zip 
VictorCervantes-picoctf@webshell:~$ ls         
challenge.zip  drop-in
VictorCervantes-picoctf@webshell:~$ cd drop-in
VictorCervantes-picoctf@webshell:~/drop-in$ git log | grep picoCTF{
Author: picoCTF{@sk_th3_1nt3rn_2c6bf174} <ops@picoctf.com>
VictorCervantes-picoctf@webshell:~/drop-in$ 

```

picoCTF{@sk_th3_1nt3rn_2c6bf174}
## Notas adicionales
- Al usar 'git log', podemos ver que se muestran muchos cambios como para poder verlos uno por uno, entonces le agregamos el comando 'grep', seguido de la palabra ' picoCTF{ ' junto con la llave { para ver el commit exacto que tenia la bandera, ya que si solo agregamos picoCTF nos imprime igual mucha información ya que todos los commits fueron realizados por el mismo usuario 'picoCTF'.

## Referencias
- https://primer.picoctf.org/#_review_of_git