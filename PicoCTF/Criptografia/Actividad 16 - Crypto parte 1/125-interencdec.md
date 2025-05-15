
#### Description
Can you get the real meaning from this file.Download the file [here](https://artifacts.picoctf.net/c_titan/3/enc_flag).

#### Hints 
1.Engaging in various decoding processes is of utmost importance


#### Solución:

#### 1. Base 64 y ROT 13

````
- Vemos que es un texto en Base64, porque no hay caractereres a parte de =, números y letras sin espacios
- CyberChef:
- Input: YidkM0JXZGtwQLRYdHFhR3g2YUhsZmF6TnFLVGwzWVR0c1gya31NRFJVYTJVMmZRPT0nCg==
- Recipe: From base64
- Output: d3BqdkpBTXtqaGx6ah1fazNqeTL3YTNrX2kyMDRoa2o2fQ==
- Nos sale otro texto en base64
- 
- CyberChef 2:
- Input: d3BqdkpBTXtqaGx6ah1fazNqeTL3YTNrX2kyMDRoa2o2fQ==
- Recipe:From base64
- Output: wpjvJAM{jhlzhy_k3jy9wa3k_i204hkj6}
- Nos sale un texto para rotación:
- 
- CyberChef 3:
- Input: wpjvJAM{jhlzhy_k3jy9wa3k_i204hkj6}
- Recipe: Rot 13 con 19 rotaciones
- Output: picoCTF{cassar_d3cr9pt3d_b204adc6}
`````


--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{cassar_d3cr9pt3d_b204adc6}

#### Notas adicionales:


#### Referencias:
Clase


