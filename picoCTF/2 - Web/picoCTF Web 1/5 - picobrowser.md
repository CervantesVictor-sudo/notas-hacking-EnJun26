# picobrowser

## Descripción
This website can be rendered only by picobrowser, go and catch the flag!

http://fickle-tempest.picoctf.net:62586

## Solución

```
VictorCervantes-academy@webshell:~$ curl -s http://fickle-tempest.picoctf.net:62586/flag -H 'User-Agent: picobrowser' | grep pico
         <!-- <strong>Title</strong> --> picobrowser!
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{p1c0_s3cr3t_ag3nt_fba5c48f}</code></p>
VictorCervantes-academy@webshell:~$ 
```

FLAG:
picoCTF{p1c0_s3cr3t_ag3nt_fba5c48f}
## Notas adicionales
- Usamos la terminal para cambiar el agente y filtrar la bandera con grep.

## Referencias
- [https://developer.mozilla.org/es/docs/Web/HTTP/Reference/Headers/User-Agent](https://developer.mozilla.org/es/docs/Web/HTTP/Reference/Headers/User-Agent)