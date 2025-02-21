
#### Description
Unzip this archive and find the file named 'uber-secret.txt'

- [Download zip file](https://artifacts.picoctf.net/c/502/files.zip)

#### Hints 
None

#### Solución:

1. Usamos el comando de find de Linux:

````
HBG-picoctf@webshell:~$ find . -name uber-secret.txt
./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
HBG-picoctf@webshell:~$ ^C
HBG-picoctf@webshell:~$ cat ./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}
HBG-picoctf@webshell:~$ 
`````

2.

````

`````

#### Pico:
picoCTF{f1nd_15_f457_ab443fd1}

#### Notas adicionales:
Clave:
find . -name uber-secret.txt

#### Referencias:



