
#### Description
This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?

#### Hints 
1. How do operating systems know what kind of file it is? (It's not just the ending!
2. Make sure to submit the flag as picoCTF{XXXXX}


#### Solución:

#### 1. Identificamos Magic Bytes, cambiamos de extensión
![[Pasted image 20250505184120.png]]

````
- Usamos xxe flag.txt | head
	- Esto es para ver los Magic Bytes y saber que tipo de arhivo es en realidad.
- Cuando vemos que no es un txt, sino un png, le cambiamos la extensión
- mv flag.txt flag.png
`````


--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{now_you_know_about_extensions}

#### Notas adicionales:
- Todos los archivos tienen un formato, 
- Magic Bytes, son como firmas que identifica el contenido de archivos
- Ya hay firmas determinadas para algunos archivos
- No importa la extensión, sino el Magic Bytes

#### Referencias:
https://www.youtube.com/watch?v=FbFpIS60M_s

