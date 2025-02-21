
#### Description
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/static)? This [BASH script](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh) might help!

#### Hints 
None

#### Solución:

1. Mediante Linux

````
HBG-picoctf@webshell:~$ ls
README.txt  ltdis.sh  static  static.ltdis.strings.txt  static.ltdis.x86_64.txt
HBG-picoctf@webshell:~$ dir
README.txt  ltdis.sh  static  static.ltdis.strings.txt  static.ltdis.x86_64.txt
HBG-picoctf@webshell:~$ cat static.ltdis.strings.txt grep | grep pico
cat: grep: No such file or directory
   1020 picoCTF{d15a5m_t34s3r_f5aeda17}
HBG-picoctf@webshell:~$ ^C
HBG-picoctf@webshell:~$ 

`````

2.

````

`````

#### Pico:
picoCTF{d15a5m_t34s3r_f5aeda17}

#### Notas adicionales:
File: Nos dice que tipo de archivo es un file
Lo que termina en sh son ejecutables.
cat nombe_archibo | grep palabra: nos permite buscar cadenas en un archivo
#### Referencias:



