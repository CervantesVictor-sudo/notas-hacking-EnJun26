# First Find

## Descripción
Unzip this archive and find the file named 'uber-secret.txt'
- **Download zip file**

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/501/files.zip
VictorCervantes-picoctf@webshell:~$ unzip files.zip 
VictorCervantes-picoctf@webshell:~$ ls
README.txt  files  files.zip
VictorCervantes-picoctf@webshell:~$ find -name uber*
./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
VictorCervantes-picoctf@webshell:~$ cat ./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{f1nd_15_f457_ab443fd1}

## Notas adicionales
- 'find' para buscar archivos y directorios, y ' -name' busca archivos por nombre exacto (distingue mayúsculas y minúsculas).

## Referencias
- 