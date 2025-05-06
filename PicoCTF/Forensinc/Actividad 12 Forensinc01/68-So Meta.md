
#### Description
Find the flag in this [picture](https://jupiter.challenges.picoctf.org/static/89b371a46702a31aa9931a2a2b12f8bf/pico_img.png).

#### Hints 
1. What does meta mean in the context of files?
2. Ever heard of metadata?

#### Solución:

#### 1. Usamos la herramiento exiftool
Esta herramienta nos ayuda a leer los metadatos de una archivo, en este caso de la imagen.
- Descargamos la imagen
- La analizamos con exiftool
![[Pasted image 20250505151106.png]]

````
comando: exiftool pico_img.png
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{s0_m3ta_eb36bf44}

#### Notas adicionales:
Los metadatos pueden contener información comprometedora, y debemos cuidar este aspecto.

#### Referencias:
https://www.youtube.com/watch?v=Govu_p-wf4I&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=15


