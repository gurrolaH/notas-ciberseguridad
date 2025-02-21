
#### Description
Unzip this archive and find the flag.

- [Download zip file](https://artifacts.picoctf.net/c/503/big-zip-files.zip)

#### Hints 
1. Can grep be instructed to look at every file in a directory and its subdirectories?


#### Solución:

1. Usando grep de Linux:

````
HBG-picoctf@webshell:~$ grep -R picoCTF
README.txt:Welcome to the picoCTF webshell!
README.txt:picoCTF challenges.
README.txt:  Extensive brute-forcing is not necessary to solve picoCTF challenges.
README.txt:- If you change your username through the picoCTF website, you will
big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}
`````

2.

````

`````

#### Pico:
picoCTF{gr3p_15_m4g1c_ef8790dc}

#### Notas adicionales:
Se uso grep -R para buscar un patrón de la carpeta donde estamos hacia abajo.

#### Referencias:



