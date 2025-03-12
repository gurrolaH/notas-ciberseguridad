
#### Description
I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/77/challenge.zip)


#### Hints 
1. Version control can help you recover files if you change or lose them!
2. Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)
3. You can 'checkout' commits to see the files inside them

#### Solución:

1. Usamos el CLI de Linux para descargar y descomprimir un zip, luego usamos el comando git log para examinar  el historial del git, de ahí sacamos la clave de un commit, por último fuimos a analizarlo para ver una bandera que antes se había creado.

````
HBG-picoctf@webshell:~/drop-in$ git log

[1]+  Stopped                 git log
HBG-picoctf@webshell:~/drop-in$ git checkout 3d5ec8a26ee7b092a1760fea18f384c35e435139
Note: switching to '3d5ec8a26ee7b092a1760fea18f384c35e435139'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 3d5ec8a create flag
HBG-picoctf@webshell:~/drop-in$ ls
message.txt
HBG-picoctf@webshell:~/drop-in$ cat message.txt 
picoCTF{s@n1t1z3_30e86d36}
`````

2.

````

`````


#### Pico:
picoCTF{s@n1t1z3_30e86d36}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=lv05wYXeouk


