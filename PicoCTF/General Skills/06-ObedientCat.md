#### Description

This file has a flag in plain sight (aka "in-the-clear"). [Download flag](https://mercury.picoctf.net/static/217686fc11d733b80be62dcfcfca6c75/flag).

#### Hints 

1. Any hints about entering a command into the Terminal (such as the next one), will start with a '$'... everything after the dollar sign will be typed (or copy and pasted) into your Terminal.
2. To get the file accessible in your shell, enter the following in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/217686fc11d733b80be62dcfcfca6c75/flag`
3. $ man cat

## Soluciones

````
3b80be62dcfcfca6c75/flagwget https://mercury.picoctf.net/static/217686fc11d733
--2025-02-13 18:35:04--  https://mercury.picoctf.net/static/217686fc11d733b80be62dcfcfca6c75/flag
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag                100%[================>]      34  --.-KB/s    in 0s      

2025-02-13 18:35:04 (18.7 MB/s) - 'flag' saved [34/34]

HBG-picoctf@webshell:~$ 
````


### PICO:
picoCTF{s4n1ty_v3r1f13d_b5aeb3dd}


