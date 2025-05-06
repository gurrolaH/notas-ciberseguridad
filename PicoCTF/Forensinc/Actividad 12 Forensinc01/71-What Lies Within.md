
#### Description
There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?

#### Hints 
1. There is data encoded somewhere... there might be an online decoder.


#### Solución:

#### 1. Usamos la herramienta Steganography Online:
![[Pasted image 20250505185628.png]]
````
- Descargamos el archivo
- Le pasamos la imagen a Steganography Online
- Le indicamos que decodificara
`````




--- 
---
#### 2. Usando ZSTEG
Es una herramienta no gráfica para esteganografía
![[Pasted image 20250505190507.png]]
````
Usamos el comando:
- zsteg -a buildings.png | grep pico
`````


#### Pico:
picoCTF{h1d1ng_1n_th3_b1t5}

#### Notas adicionales:
- La esteganografía es más útil cuando va de la mano de la encriptación
- La esteganografía es para  ocultar información
- Hay herramientas de esteganografía, por eso bueno además codificar

#### Referencias:
https://www.youtube.com/watch?v=bFUB-USG3sw


