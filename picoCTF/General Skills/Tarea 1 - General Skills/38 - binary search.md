# Binary search

## Descripción
Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!
You download the challenge files here: challenge.zip
`ssh -p 54508 ctf-player@atlas.picoctf.net`Using the password `1db87a14`. Accept the fingerprint with `yes`, and `ls` once connected to begin. Remember, in a shell, passwords are hidden!

## Solución
```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c_atlas/19/challenge.zip
VictorCervantes-picoctf@webshell:~$ unzip challenge.zip 
VictorCervantes-picoctf@webshell:~$ ls
challenge.zip  home
VictorCervantes-picoctf@webshell:~$ cd home/
VictorCervantes-picoctf@webshell:~/home$ cd ctf-player/
VictorCervantes-picoctf@webshell:~/home/ctf-player$ cd drop-in/
VictorCervantes-picoctf@webshell:~/home/ctf-player/drop-in$ ls
guessing_game.sh
VictorCervantes-picoctf@webshell:~/home/ctf-player/drop-in$ ssh -p 54508 ctf-player@atlas.picoctf.net
The authenticity of host '[atlas.picoctf.net]:54508 ([18.217.83.136]:54508)' can't be established.
ED25519 key fingerprint is SHA256:M8hXanE8l/Yzfs8iuxNsuFL4vCzCKEIlM/3hpO13tfQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[atlas.picoctf.net]:54508' (ED25519) to the list of known hosts.
ctf-player@atlas.picoctf.net's password: 
Welcome to the Binary Search Game!
Enter your guess: 500
Lower! Try again.
Enter your guess: 250
Lower! Try again.
Enter your guess: 125
Lower! Try again.
Enter your guess: 75
Lower! Try again.
Enter your guess: 30
Higher! Try again.
Enter your guess: 55
Higher! Try again.
Enter your guess: 65
Higher! Try again.
Enter your guess: 70
Higher! Try again.
Enter your guess: 73
Higher! Try again.
Enter your guess: 74
Congratulations! You guessed the correct number: 74
Here's your flag: picoCTF{g00d_gu355_1597707f}
Connection to atlas.picoctf.net closed.
VictorCervantes-picoctf@webshell:~/home/ctf-player/drop-in$ 

```

picoCTF{g00d_gu355_1597707f}

## Notas adicionales
- 

## Referencias
- 