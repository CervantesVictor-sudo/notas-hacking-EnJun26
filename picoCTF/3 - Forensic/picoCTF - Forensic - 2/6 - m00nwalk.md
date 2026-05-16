# m00nwalk

## Descripción
Decode this [message](https://challenge-files.picoctf.net/c_fickle_tempest/816c75fc4b45dfc4ab4c4caad4ac738a3e0cfb3825fedda2a753eb5360c477bb/message.wav) from the moon.

## Solución

FLAG:

picoCTF{beep_boop_im_in_space}


## Notas adicionales
- Se utilizó una herramienta para decodificar el audio la cual se extrajo de github con el siguiente comando
```
$ git clone https://github.com/colaclanth/sstv.git

$ python setup.py install
```

- Luego se usó el siguiente comando

```
sstv -d message.wav.1 -o result.png
```
## Referencias
- https://github.com/colaclanth/sstv