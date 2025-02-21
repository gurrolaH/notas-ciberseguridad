
#### Description

Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings) without running it?


#### Hints 
https://linux.die.net/man/1/strings



#### Solución:

1.- Linux usando el comando strings.

````
HBG-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
--2025-02-20 22:07:28--  https://jupiter.challenges.picoctf.org/static/fae9ac5267cd6e44124e559b901df177/strings
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 776032 (758K) [application/octet-stream]
Saving to: 'strings.1'

strings.1                                   100%[===========================================================================================>] 757.84K  1.86MB/s    in 0.4s    

2025-02-20 22:07:29 (1.86 MB/s) - 'strings.1' saved [776032/776032]

HBG-picoctf@webshell:~$ dir
README.txt  datos  strings  strings.1
HBG-picoctf@webshell:~$ rm strings.1
HBG-picoctf@webshell:~$ dir
README.txt  datos  strings
HBG-picoctf@webshell:~$ strings strings | grep pico
picoCTF{5tRIng5_1T_7f766a23}
HBG-picoctf@webshell:~$ 
`````

2.

````

`````

#### Notas adicionales:
No se puede leer archivos ejecutables con el comando CAT


#### Referencias:



