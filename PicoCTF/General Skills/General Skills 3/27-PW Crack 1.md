
#### Description
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/12/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/12/level1.flag.txt.enc) in the same directory too.
#### Hints 
1. To view the file in the webshell, do: `$ nano level1.py`
2. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
3. The `str_xor` function does not need to be reverse engineered for this challenge.


#### Solución:

1. Usamos wget, luego nano para saber el pin, por último lo corrimos con pyhton3.

````
HBG-picoctf@webshell:~$ ls
README.txt  code.py  codebook.txt  level1.flag.txt.enc  level1.py
HBG-picoctf@webshell:~$ nano level1.flag.txt.enc 
HBG-picoctf@webshell:~$ nano level1.py 
HBG-picoctf@webshell:~$ python3 level1.py 
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}
`````

2.

````

`````


#### Pico:
picoCTF{545h_r1ng1ng_1b2fd683}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=VPCXVCI2FAA

