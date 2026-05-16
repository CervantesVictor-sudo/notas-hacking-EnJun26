# logon

## Descripción
The factory is hiding things from all of its users.

Can you login as Joe and find what they've been looking at? http://fickle-tempest.picoctf.net:49943

## Solución
Usando cookie editor

https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search

Ingresamos a la página como:
- admin
- 1234

Como admin tiene cookies False con cookie editor las cambiamos a True y recargamos la página

Flag: 
picoCTF{th3_c0nsp1r4cy_l1v3s_4d184b0d}


## Notas adicionales
- 

## Referencias
- [https://developer.mozilla.org/es/docs/Web/HTTP/Reference/Headers](https://developer.mozilla.org/es/docs/Web/HTTP/Reference/Headers)

- [https://developer.mozilla.org/en-US/docs/Glossary/Request_header](https://developer.mozilla.org/en-US/docs/Glossary/Request_header)

- [https://developer.mozilla.org/es/docs/Web/HTTP/Guides/Cookies](https://developer.mozilla.org/es/docs/Web/HTTP/Guides/Cookies)