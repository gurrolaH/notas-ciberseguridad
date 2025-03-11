#### Description
Fix the syntax error in this Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/25/fixme1.py)

#### Hints 
1. Indentation is very meaningful in Python
2. To view the file in the webshell, do: `$ nano fixme1.py`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.


#### Solución:

1. Usamos un editor que es nano para corregir un script de python, en una identación. Luego lo corrimos con python3.

````
HBG-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/25/fixme1.py
--2025-03-11 11:26:39--  https://artifacts.picoctf.net/c/25/fixme1.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.128, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 837 [application/octet-stream]
Saving to: 'fixme1.py'

fixme1.py                100%[===============================>]     837  --.-KB/s    in 0s      

2025-03-11 11:26:39 (383 MB/s) - 'fixme1.py' saved [837/837]

HBG-picoctf@webshell:~$ ls
README.txt  code.py  codebook.txt  fixme1.py
HBG-picoctf@webshell:~$ nano fixme1.py 
HBG-picoctf@webshell:~$ python3 fixme1.py 
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_6a476c8f}
`````

2.

````

`````


#### Pico:
picoCTF{1nd3nt1ty_cr1515_6a476c8f}

#### Notas adicionales:


#### Referencias:
CLI de Linux.


