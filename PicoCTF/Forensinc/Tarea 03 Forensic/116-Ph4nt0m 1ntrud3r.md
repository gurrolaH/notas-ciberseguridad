
#### Description
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/a917f567b9cc0f1a730a7801b309955df4d2234a8114326857b9759e9e5d0453/myNetworkTraffic.pcap) and try to get the flag.

#### Hints 
1. Filter your packets to narrow down your search.
2. Attacks were done in timely manner.
3. Time is essential

#### Solución:

#### 1. Usamo WireShark

````
wget https://challenge-files.picoctf.net/c_verbal_slee
NetworkTraffic.pcap
cler
clear
ls
wireshark myNetworkTraffic.pcap

Dentro de Wireshark:
- Filtramos de longitud 4 y 12
- Filtramos por tiempo
- Mostramos los Bytes de los paquetes
- Que lo decodifique de base 64
- Vamos mostrando los paquetes y formando la flag
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_959f50d3}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=_YKC5Smffeg

