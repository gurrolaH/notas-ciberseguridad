#### Description
Decode this [message](https://jupiter.challenges.picoctf.org/static/d6fcea5e3c6433680ea4f914e24fab61/message.wav) from the moon.

#### Hints 
1. How did pictures from the moon landing get sent back to Earth?
2. What is the CMU mascot?, that might help select a RX option


#### Solución:

#### 1. Usamos la herramienta sstv

````
- Descargamos el archivo
- Era un wav, pero no tenía nada coherente
- Descargamos sstv desde un repo git
- Usamo la herramienta sstv con el archivo wav
- Como resultado nos lo decodificó a un png.
- La bandera estaba en el png.
`````
![[Pasted image 20250409074413.png]]
````Imagen con el history de los comandos ejecutados.
`````


--- 
---
#### 2.

````

`````


#### Pico:
![[Pasted image 20250409074705.png]]
picoCTF{beep_boop_im_in_space}

#### Notas adicionales:
Se puede codificar audios y en realidad sean imágenes.

#### Referencias:
https://www.youtube.com/watch?v=UyLTEpAz6eE&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=19


