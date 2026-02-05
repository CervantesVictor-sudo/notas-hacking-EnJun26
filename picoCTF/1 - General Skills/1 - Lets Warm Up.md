## Descripción
If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

# Solución

### Solución 1
- Usando cyberchef
- https://gchq.github.io/CyberChef/#recipe=From_Hex('0x')&input=MHg3MA
### Solución 2
- Usando python
```
- >>> int(0x70)
112
>>> chr(112)
'p'
>>> ord('p')
112
>>> 
```
## Notas adicionales
- Usamos la pagina de cyberchef para resolver el reto
- Se uso la terminal de Pico para resolver el reto mediante Python
## Referencias
- https://gchq.github.io/CyberChef/