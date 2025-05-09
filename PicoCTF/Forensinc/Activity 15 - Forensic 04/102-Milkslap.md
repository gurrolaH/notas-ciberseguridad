
#### Description
[🥛](http://mercury.picoctf.net:48380/)

#### Hints 
Look at the problem category


#### Solución: 
![[Pasted image 20250507234456.png]]
#### 1. Usamos "zsteg"
Que detecta datos ocultos en archivos PNG y BMP

````
1. Inspeccionamos la página web

2. Ubicamos la pestaña "source"

3.Pero antes para que funcionara:
- export RUBY_THREAD_VM_STACK_SIZE=5000000

4. Descargamos la imágen y aplicamos:
- zsteg concat_v.png | grep "picocTF
`````




--- 
---
#### 2.

````

`````


#### Pico:
picocTF{img3_m4n1pu14t10n_s14p5}

#### Notas adicionales:
- zsteg, herramienta forensic

#### Referencias:
https://www.youtube.com/watch?v=QyjkyWEDHII

