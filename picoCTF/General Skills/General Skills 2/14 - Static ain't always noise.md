# Static ain't always noise

## Descripción
Can you look at the data in this binary? The bash script might help!

## Solución
```
VictorCervantes-picoctf@webshell:~$ ls
README.txt  ltdis.sh  static
VictorCervantes-picoctf@webshell:~$ file *
README.txt: ASCII text, with escape sequences
ltdis.sh:   Bourne-Again shell script, ASCII text executable
static:     ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=9a00d4dca6b92d22aa0cd1fceffa4ed7495b8534, for GNU/Linux 3.2.0, not stripped
VictorCervantes-picoctf@webshell:~$ ./ltdis.sh
-bash: ./ltdis.sh: Permission denied
VictorCervantes-picoctf@webshell:~$ chmod +x ltdis.sh
VictorCervantes-picoctf@webshell:~$ ./ltdis.sh
Attempting disassembly of  ...
objdump: 'a.out': No such file
objdump: section '.text' mentioned in a -j option, but not found in any input file
Disassembly failed!
Usage: ltdis.sh <program-file>
Bye!
VictorCervantes-picoctf@webshell:~$ ./ltdis.sh static
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
VictorCervantes-picoctf@webshell:~$ ls
README.txt  static                    static.ltdis.x86_64.txt
ltdis.sh    static.ltdis.strings.txt
VictorCervantes-picoctf@webshell:~$ strings static | grep pico
picoCTF{d15a5m_t34s3r_20335e41}

```
picoCTF{d15a5m_t34s3r_20335e41}
## Notas adicionales
- 

## Referencias
- 