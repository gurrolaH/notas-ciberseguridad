
#### Description
Every file gets a flag.The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/256/flag.png).

#### Hints 
(None)


#### Solución:

#### 1. Usamos binwalk

````
Dimwalk flag.png -e
ls
cd _flag.png.extracted
ls
binwalk flag.png -e
clear
cd secret
la
binwalk flag.png -e
ls
cd _flag.png.extracted
ls 
cd ..
ls
clear
pwd
cd ..
ls
cd secret
ls
open flag.png
`````

![[Pasted image 20250515161149.png]]


--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{Hidding_An_imag3_within_an_ima9e_85804ab8}

#### Notas adicionales:


#### Referencias:



