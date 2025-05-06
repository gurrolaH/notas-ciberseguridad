
#### Description
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/2e739f9e0dc9f4c1556ea6b033c3ec8e/Forensics%20is%20fun.pptm)

#### Hints 
None

#### Solución:

#### 1. Utilizamos el explorador de archivos de VSC
![[Pasted image 20250506084103.png]]
````
1. Utilizamos el explorador de archivos de Visual Studio Code, ya que es más gráfico.
2. Analizando ubicamos un archivo llamado hidden.
3. Lo abrimos y tenía una cadene en base 64 y con espacios
4. Le aplicamos un:
	- echo Z m x h Z z o g c G l j b O N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q | tr -d " " | base64 -d
5. Obtuvimos la bandera
`````




--- 
---
#### 2.

````

`````


#### Pico:
picocTF{0id_u_kn0w_ppts_r_zip5}

#### Notas adicionales:
- VSC posee un explorador muy intuitivo


#### Referencias:
https://www.youtube.com/watch?v=CsCeOp9PFGs&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=28


