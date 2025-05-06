
#### Description
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

#### Hints 
1. Try using a tool like Wireshark.
2. How can you decrypt the TLS stream?


#### Solución:

#### 1. Se usa Wireshark
Se usan las propiedades de Wireshark para agregar una llave privada, después de esto se puede desencriptar los paqutes PCAP.
![[Pasted image 20250505231650.png]]


````
1. Nos vamos a EDIT
	1. Preferences
	2. Protocolos
	3. TLS
2. Le damos la ubicación de la llave RSA
3. Se desencriptan los paqutes
4. Hacemos una búsqueda en EDIT
	1. find next
	2. Packet details
	3. Strings
		1. Buscamos "picoCTF"
`````



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{nongshim.shrimp.crackers}


#### Notas adicionales:
- TLS: Transportar información segura a través de la red, privacidad, etc, usando criptografía
- Viene de SSL
- TLS es para la arquitectura cliente servidor


#### Referencias:
https://www.youtube.com/watch?v=9uflLPoETOc&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=24


