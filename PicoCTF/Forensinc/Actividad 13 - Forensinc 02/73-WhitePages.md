
#### Description
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/95be9526e162185c741259a75dffa0ab/whitepages.txt) is all blank!

#### Hints 
None


#### Solución:

#### 1. Decodificamos el texto Unicode

````
- Instalamos en un ambiente virtual en pwntools
- Hicimos un script en python que nos ayudará a leer los datos en la codificación que estuvieramos.
	- from pwn import *
file = open('whitepages.txt', 'rb')
data = bytearray(file.read())
data = data.replace(b'\xe2\x80\x83', b'0')
data = data.replace(b'\x20', b'1')
data = (data.decode('ascii'))
data = unbits(data)
print(data)

- Se asumió que había 1 y 0. 
	- Eran dos codificaciones.
- Reemplazamos por 0 y 1
- Imprimos en decodificación ascii
`````
![[Pasted image 20250409164507.png]]



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{not_all_spaces_are_created_equal_7100860b0fa779a5bd8ce29f24f586dc}
![[Pasted image 20250409164705.png]]

#### Notas adicionales:
Puede haber codificaciones en Unicode y si son dos codificaciones puede que se binario.

#### Referencias:
https://www.youtube.com/watch?v=427HDV7tzow&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=20


