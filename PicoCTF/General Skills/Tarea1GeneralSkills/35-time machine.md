
#### Description
What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/68/challenge.zip)


#### Hints 
1. The `cat` command will let you read a file, but that won't help you here!
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).}
3. When committing a file with git, a message can (and should) be included.

#### Solución:

1. Desde el CLI descargamos el zip, luego lo descomprimimos con unzip, y con git log descubrimos la descripción que era la flag.

````
commit 705ff639b7846418603a3272ab54536e01e3dc43 (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:10:36 2024 +0000

    picoCTF{t1m3m@ch1n3_b476ca06}


commit 705ff639b7846418603a3272ab54536e01e3dc43 (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:10:36 2024 +0000

    picoCTF{t1m3m@ch1n3_b476ca06}
`````

2.

````

`````


#### Pico:
picoCTF{t1m3m@ch1n3_b476ca06}

#### Notas adicionales:


#### Referencias:
https://primer.picoctf.org/#_git_version_control


