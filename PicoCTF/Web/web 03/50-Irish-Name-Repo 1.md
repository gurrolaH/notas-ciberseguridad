
#### Description
`https://jupiter.challenges.picoctf.org/problem/39720/` ([link](https://jupiter.challenges.picoctf.org/problem/39720/)) or http://jupiter.challenges.picoctf.org:39720. Do you think you can log us in? Try to see if you can login!

#### Hints 
1. There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?
2. Try to think about how the website verifies your login.

#### Solución:

1.Usamos el inspector del navegador.

````
Al usar el inspector del navegador descubrimos qué fue lo que fue lo que se haces al darle click  a un botón de acceder.
Ya que sabemos que hace enviamos algún valor que deba recibir.
`````
![[Pasted image 20250326234933.png]]




2. Para la solución dos usamos la consola:

````
Usamos Curl y cambiamos .php y usamos -d para pasarle entre comillas el usario y la password.
`````
![[Pasted image 20250327000237.png]]






#### Pico:

picoCTF{s0m3_SQL_c218b685}
![[Pasted image 20250326234838.png]]




#### Notas adicionales:
Se usa inyección SQL.

#### Referencias:



