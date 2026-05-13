# Repetitions

## Descripción
Can you make sense of this file?
Download the file **here**.

## Solución
Primero, obtenemos la cadena del archivo:
```
VictorCervantes-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/473/enc_flag
VictorCervantes-picoctf@webshell:~$ file enc_flag 
enc_flag: ASCII text
VictorCervantes-picoctf@webshell:~$ cat enc_flag 
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbHBWV0VKVVZGWm9RMlZzV2tWUmJFNVNDbUpXV25wWmExSmhWMGRHZEdWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==
VictorCervantes-picoctf@webshell:~$

```
Despues, tenemos dos opciones: la primera, en CiberChef agregamos 6 veces el 'from base64' y escribimos el texto que nos dió el archivo
- https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)From_Base64('A-Za-z0-9%2B/%3D',true,false)From_Base64('A-Za-z0-9%2B/%3D',true,false)From_Base64('A-Za-z0-9%2B/%3D',true,false)From_Base64('A-Za-z0-9%2B/%3D',true,false)From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=Vm1wR1UxRXlSWGxVV0d4VFlteEtWVll3WkZOV2JHeHlWMjFHVjFKdGVEQlViRnBQWVd4S2RGVnNhRnBXVmxVeFdWWmFTMVpXV25WaApSbVJYWld0YWIxZFdXbXRTTWs1eVRsWldXQXBpVlZwVVZtMTBkMVZXWkZkVmEyUnBZbFphV0ZadE5WZFZaM0JwVTBWS2VsZFdVa05rCk1sWlhWbGhvV0dKWVFrOVZiRkpYVTBaa2NWUnVUbGRhTTBKWlZXcEdTMlZXV2tkYVNHUlhDazFzV25wV1YzaGhWbTFLUms1WE9WVlcKVmtwRVZHeGFZVmRGTVZoU2JIQldWMFZLVlZaR1dtOVJNbFp6VjJ0V1VtSkZOVk5EYlVwWFYyNXdXbUV4U21oV01HUkhaRWRXUmxacwphR2tLWWxScmVsWkVSbGRVTWtwelVXeFdUbEpZVGt4RFp6MDlDZz09
La segunda, seria directamente en la terminal:
```
VictorCervantes-picoctf@webshell:~$ cat enc_flag | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_dfe803c6}
VictorCervantes-picoctf@webshell:~$ 

```
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_dfe803c6}

## Notas adicionales
- 

## Referencias
- 