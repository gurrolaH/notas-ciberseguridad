
#### Description
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

#### Hints 
None


#### Solución:

#### 1. Usamos scappy:

````
- Descargamos el paquete y vemos son paquetes
- Los analizamos con wire shark y vemos que hay mucho UDP
- Seguimos los UDP y vemos que hay pistas de inicio y de fin.
- Hay una codificación en los puertos.
- Instalamos scappy en un ambiente virtualizado.
- Luego hicimos un script en python y que usaba la librería scapy.all.
	
- from scapy.all import *

packets = rdpcap('capture.pcap')

flag = ''

# Filtrado de paquetes:
for cadaPaquete in packets:
    if UDP in cadaPaquete and cadaPaquete[UDP].dport == 22:
        if cadaPaquete[UDP].sport > 5000:  # Para verificar que es el cifrado
            flag += chr(cadaPaquete[UDP].sport - 5000)

print(flag)



- Obtuvimos la bandera al poder codificar en ascii lo que nos indicaba cada puerto n - 5000.
`````


![[Pasted image 20250410004520.png]]

--- 
---
#### 2.

````

`````


#### Pico:
![[Pasted image 20250410004329.png]]

#### Notas adicionales:
Se puede mandar información o ascii encriptado en puertos de net.

#### Referencias:
https://chat.deepseek.com/a/chat/s/96b69907-fd71-4bce-8776-99f0070e3802


