
#### Description
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/213/disk.flag.img.gz)

#### Hints 
(None)


#### Solución: Usando comandos de 

#### 1. Slouth Kit

````
wget https://artifacts.picoctf.net/c/213/disk.flag.img.gz
gzip -d disk.flag.img.gz
ls
mmls disk.flag.img

fls disk.flag.img -o 411648
fls disk.flag.img -o 411648 472

icat disk.flag.img -o 411648 1782
icat disk.flag.img -o 411648 1785
icat disk.flag.img -o 411648 1875

icat disk.flag.img -o 411648 1782 > flag.txt.enc
icat disk.flag.img -o 411648 1875

openssl aes256 -d -salt -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567

cat flag.txt
`````



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{h4un71ng_p457_5113beab}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=rXY4BCtonJs


