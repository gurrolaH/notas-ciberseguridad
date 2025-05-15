
#### Description
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg)

#### Hints 
1. Look at the details of the file
2. Make sure to submit the flag as picoCTF{XXXXX}

#### Solución:

#### 1. Usamos exiftool para ver los metadatos

````
wget https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg
ls
ls -la cat.jpg
file cat.jpg
exiftool cat.jpg
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF[the_m3tadata_1s_modified]


#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=uG42AMp0XHU


