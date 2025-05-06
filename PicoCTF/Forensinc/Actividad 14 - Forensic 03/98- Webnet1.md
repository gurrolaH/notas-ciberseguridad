
#### Description
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.

#### Hints 
1. Try using a tool like Wireshark.
2. How can you decrypt the TLS stream?

#### Solución:

#### 1. Usamo Wireshark
![[Pasted image 20250505233319.png]]
````
1. Nos vamos a EDIT
	1. Preferences
	2. Protocolos
	3. TLS
2. Le damos la ubicación de la llave RSA
3. Se desencriptan los paqutes
4. Cuado se desencriptan vemos que se hace la descarga de una imagen
5. La guardamos en disco
6. Le hacemos un
	1. strings vulture.jpg -n15 | grep "picoCTF"
7. Obtenemos la flag
`````




--- 
---
#### 2. Usando Whireshark

````
En lugar de descargar la imagen en el disco, se hace directo un seguimieto del stream de los paqutes, llegamos a la imagen, en los datos de la imagen que se descarga
`````


#### Pico:
picoCTF{honey.roasted.peanuts}

#### Notas adicionales:
- Se puede usar también el ssldump

#### Referencias:
https://www.youtube.com/watch?v=Ym3i79nEHjw&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=25

