
#### Description
Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/1e4bd835ad3e7fe776d49e7b8cc280c1/server.py) [http://mercury.picoctf.net:35697/](http://mercury.picoctf.net:35697/)

#### Hints 
1. How secure is a flask cookie?

#### Solución:

#### 1. Alteramos la cookie con flask-unsign:

````
- Primero vimos que hay cookies en el sitio web
- Decodificamos la cookie para darnos una idea de qué puede ser la clave.
- Hicimos un ataque de fuerza bruta con flask-unsign y una wordlist.
- Alteramos la cookie con la palabra clave.
`````
![[Pasted image 20250407174705.png]]


![[Pasted image 20250407174641.png]]

![[Pasted image 20250407181635.png]]


![[Pasted image 20250407181702.png]]


![[Pasted image 20250407181923.png]]

![[Pasted image 20250407182205.png]]







--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{pwn_4ll_th3_cook1E5_22fe0842}
![[Pasted image 20250407182252.png]]



#### Notas adicionales:
No debemos fiarnos de que por usar algún framework ya es todo seguro, debemos asegurarnos de las cookies no puedan ser alteradas, o que se pueda descubrir las claves.

#### Referencias:
https://www.youtube.com/watch?v=ufs1xqSQCUM


