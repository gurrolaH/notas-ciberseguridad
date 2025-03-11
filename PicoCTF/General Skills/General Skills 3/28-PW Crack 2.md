
#### Description
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/15/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/15/level2.flag.txt.enc) in the same directory too.

#### Hints 
1. Does that encoding look familiar?
2. The `str_xor` function does not need to be reverse engineered for this challenge.

#### Solución:

1. Con el CLI descargué el archivo y con nano lo leí, luego con Cyberchef lo desencripté usando de HEX

````
HBG-picoctf@webshell:~$ nano level2.py 
HBG-picoctf@webshell:~$ pyhton3 level2.py 
-bash: pyhton3: command not found
HBG-picoctf@webshell:~$ python3 level2.py  
Please enter correct password for flag: 39ce
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_502ec42e}


Parte de CYBERCHEF:
Entrada: chr(0x33) + chr(0x39) + chr(0x63) + chr(0x65)
Salida: 39ce
Receta: De Hex
`````

2.

````

`````


#### Pico:
picoCTF{tr45h_51ng1ng_502ec42e}

#### Notas adicionales:
3+9+c+e
39ce

#### Referencias:
https://gchq.github.io/CyberChef/#recipe=From_Hex('0x')&input=MHg2NQ
