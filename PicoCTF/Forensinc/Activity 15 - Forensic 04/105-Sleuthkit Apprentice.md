
#### Description
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

- [Download compressed disk image](https://artifacts.picoctf.net/c/137/disk.flag.img.gz)

#### Hints 
(None)


#### Solución:

#### 1. Usamos los siguientes comandos Sleuth Kit

````
wget https://artifacts.picoctf.net/c/137/disk.flag.img.gz
ls
gzip -d disk.flag.img.gz
ls
ls -lah
srch_strings disk.flag.img | grep pico
mmls disk.flag.img
fls disk.flag.img -o 360448
find -type d -name "pico"
fls disk.flag.img -o 360448 -r | grep flag
icat disk.flag.img -o 360448 2371
`````



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{by73_5urf3r_adac6cb4}

#### Notas adicionales:


#### Referencias:
Clase

