
#### Description
Someone's commits seems to be preventing the program from working. Who is it?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/158/challenge.zip)

#### Hints 
1. In collaborative projects, many users can make many changes. How can you see the changes within one file?
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
3. You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.


#### Solución:

1. Solo use git log y busqué la flag de manera manual

````
HBG-picoctf@webshell:~/drop-in$ git log

[3]+  Stopped                 git log
HBG-picoctf@webshell:~/drop-in$ 


commit 8c83358c32daee3f8b597d2b853c1d1966b23f0a
Author: picoCTF{@sk_th3_1nt3rn_2c6bf174} <ops@picoctf.com>
Date:   Tue Mar 12 00:07:11 2024 +0000

    optimize file size of prod code
`````

2. Para no hacer la búsqueda manual, sino con ayud:

````
git log | grep picoCTF{@
`````


#### Pico:
picoCTF{@sk_th3_1nt3rn_2c6bf174}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=8Q8jiZHGfJI



