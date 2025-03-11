
#### Description
Fix the syntax error in the Python script to print the flag.[Download Python script](https://artifacts.picoctf.net/c/5/fixme2.py)

#### Hints 
1. Are equality and assignment the same symbol?
2. To view the file in the webshell, do: `$ nano fixme2.py`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.
#### Solución:


1. Usamos CLI de linux para descargar, nano para arreglar el script. luego lo corrimos con python3.

````
HBG-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/5/fixme2.py
--2025-03-11 11:29:07--  https://artifacts.picoctf.net/c/5/fixme2.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.16, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1029 (1.0K) [application/octet-stream]
Saving to: 'fixme2.py'

fixme2.py                100%[===============================>]   1.00K  --.-KB/s    in 0s      

2025-03-11 11:29:07 (44.2 MB/s) - 'fixme2.py' saved [1029/1029]

HBG-picoctf@webshell:~$ ls
README.txt  code.py  codebook.txt  fixme1.py  fixme2.py
HBG-picoctf@webshell:~$ nano fixme2.py 
HBG-picoctf@webshell:~$ python3 fixme2.py 
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}
`````

2.

````

`````


#### Pico:
picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}

#### Notas adicionales:


#### Referencias:
Linux CLI