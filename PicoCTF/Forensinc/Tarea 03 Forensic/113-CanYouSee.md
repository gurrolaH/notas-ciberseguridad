
#### Description
How about some hide and seek?Download this file [here](https://artifacts.picoctf.net/c_titan/4/unknown.zip).

#### Hints 
1. How can you view the information about the picture?
2. If something isn't in the expected form, maybe it deserves attention?

#### Solución:

#### 1. Obtenemos de exiftool la flag

````
wget https://artifacts.picoctf.net/c_titan/4/unknown.zip
ls
gzip -d unknown.zip
unzip unknown.zip
ls
exiftool ukn_reality.jpg
clear
base64 -d "cGljbONURntNRTc0RDQ3QV9ISUREM05fZGVjYTA2ZmJ9Cg=="
clear
echo "cGljbONURntNRTc0RDQ3QV9ISUREM05fZGVjYTA2ZmJ9Cg==" | base64 -d
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{ME74D47A_HIDD3N_deca06fb}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=gULOheSTfmk


