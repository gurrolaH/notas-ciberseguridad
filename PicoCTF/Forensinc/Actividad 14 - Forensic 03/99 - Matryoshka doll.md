
#### Description
Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/1b70cffdd2f05427fff97d13c496963f/dolls.jpg)

#### Hints 
1. Wait, you can hide files inside files? But how do you find them?
2. Make sure to submit the flag as picoCTF{XXXXX}

#### Solución:
![[Pasted image 20250506073548.png]]

#### 1. Usamos el comando "binwalk"

````
Usamos la herramienta binwalk:
1. Aplicamos binwalk a la imagen
	- Vemos que hay un arhivo compimido dentro de la imagen
2. Aplicamos un binwalk -e a la imágen, para hacer la extracción del archivo comprimido.
	- Se nos agregar una subcarpeta, que es la que había comprimido dentro de la image.
3. Repetimos el proceso en diferentes ocasiones
	- Después de 4 extracciones, ya no hay carpetas, sino un TXT con la flag
`````



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{bf6acf878dcbd752f4721e41b1b1b66b}

#### Notas adicionales:
- Puede haber archivos comprimidos en las imágenes

#### Referencias:
https://www.youtube.com/watch?v=NkbtA7x5aVI&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=26


