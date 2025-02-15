RETO: REPETITIONS

Descripcion:
Can you make sense of this file?

Solucion: 
Al iniciar el reto me di cuenta que tenia una tag de Base64... con lo cual ya me daba una idea de por donde hiba el reto... 

Al descargar el archivo y ver que contenia, me percate que era base 64, pero demasiado largo diria yo, le aplique una primera decodificacion y me di cuenta que se reducio el largo...

Con lo cual fui aplicando una decodificacion mas hasta que poco a poco se fue viendo la flag:
```
┌──(kali㉿kali)-[~]
└─$ cat enc_flag       
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbFZhTTBKUFdXdGtlbVF4V2tkWGJYUllDbUY2UWpSWmEyaFRWakpHZEdWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d 
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlVaM0JPWWtkemQxWkdXbXRYCmF6QjRZa2hTVjJGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d -W 0
base64: invalid option -- 'W'
Try 'base64 --help' for more information.
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d --wrap=0
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlVaM0JPWWtkemQxWkdXbXRYCmF6QjRZa2hTVjJGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d -i      
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlVaM0JPWWtkemQxWkdXbXRYCmF6QjRZa2hTVjJGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d -i | base64 -d             
V1RCa2MyRnRTWGRVYkZaVFltNVNjRmRXYUU5aVJUVnhWVzFhYVdGck5UWmFSVkpQWVRGbmVWVnVR
bHBsYTBweVUxWmpNRTVHWjNsVgpXR1JyVFdwV2VsUlZVbE5oTURCNVZXMWFUZ3BOYkdzd1ZGWmtX
azB4YkhSV2FteEVXbm93T1VOblBUMEsK
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d -i | base64 -d  | base64 -d | base64 -d 
Y0dsamIwTlVSbnRpWVhObE5qUmZiak56ZEROa1gyUnBZekJrSVc0NFgyUXdkMjVzTURSa00yUmZN
Mlk0TVdZM1ltVjlDZz09Cg==
                                                                                                                                                                       
┌──(kali㉿kali)-[~]
└─$ cat enc_flag | base64 -d -i | base64 -d  | base64 -d | base64 -d | base64 -d | base64 -d 
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_3f81f7be}
```

