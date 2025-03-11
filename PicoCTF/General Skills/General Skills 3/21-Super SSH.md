
#### Description
Using a Secure Shell (SSH) is going to be pretty important.

Additional details will be available after launching your challenge instance.

Using a Secure Shell (SSH) is going to be pretty important.Can you `ssh` as `ctf-player` to `titan.picoctf.net` at port `56949` to get the flag?You'll also need the password `1db87a14`. If asked, accept the fingerprint with `yes`.If your device doesn't have a shell, you can use: [https://webshell.picoctf.org](https://webshell.picoctf.org/)If you're not sure what a shell is, check out our Primer: [https://primer.picoctf.com/#_the_shell](https://primer.picoctf.com/#_the_shell)

#### Hints 
This challenge launches an instance on demand.  
Its current status is: `NOT_RUNNING`

1. [https://linux.die.net/man/1/ssh](https://linux.die.net/man/1/ssh)
2. You can try logging in 'as' someone with `<user>`@titan.picoctf.net
3. How could you specify the port?
4. Remember, passwords are hidden when typed into the shell


#### Solución:

1. Usamo ssh del CLI de Linux.

````
HBG-picoctf@webshell:~$ ssh ctf-player@titan.picoctf.net -p 52670 
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_45a48857}
Connection to titan.picoctf.net closed.
`````

2.

````

`````


#### Pico:
picoCTF{s3cur3_c0nn3ct10n_45a48857}

#### Notas adicionales:
No podía aunque usaba ssh, porque no especificaba como el nombre del usuario.

#### Referencias:
https://www.youtube.com/watch?v=u-nNvwlXDL4


