# Based

## Descripción
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337?Connect with nc fickle-tempest.picoctf.net 64355.

## Solución
- https://gchq.github.io/CyberChef/#recipe=From_Binary('Space',8)&input=MDExMDAwMTEgMDExMDEwMDAgMDExMDAwMDEgMDExMDEwMDEgMDExMTAwMTA
- https://gchq.github.io/CyberChef/#recipe=Find_/_Replace(%7B'option':'Regex','string':'o'%7D,'',true,false,true,false)From_Octal('Space')&input=bzE0MSBvMTU2IG8xNTEgbzE1NSBvMTQxIG8xNjQgbzE1MSBvMTU3IG8xNTY
- https://gchq.github.io/CyberChef/#recipe=From_Hex('Auto')&input=NmM2OTZkNjU
```
VictorCervantes-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 64355
Let us see how data is stored
chair
Please give the 01100011 01101000 01100001 01101001 01110010 as a word.
...
you have 45 seconds.....

Input:
chair
Please give me the  o141 o156 o151 o155 o141 o164 o151 o157 o156 as a word.
Input:
animation
Please give me the 6c696d65 as a word.
Input:
lime
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_aa2bA794}

VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{learning_about_converting_values_aa2bA794}
## Notas adicionales
- Se usaron 3 pestañas de CiberChef para hacer las conversiones: la primera fue de binario, la segunda se usó 'find / replace' para quitar la "o" y obtener la palabra de octal, y al final se usó de hexadecimal.

## Referencias
- https://gchq.github.io/CyberChef/

