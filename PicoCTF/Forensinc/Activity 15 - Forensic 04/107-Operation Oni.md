
#### Description
Download this disk image, find the key and log into the remote machine.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

Additional details will be available after launching your challenge instance.

#### Hints 
(None)

#### Solución:

#### 1. Usando herramientas de Slouth Kit

````
wget https://artifacts.picoctf.net/c/70/disk.img.gz
ls
gzip -d disk.img.gz

mmls disk.img
fls disk.img -o 206848
fls disk.img -o 206848 470
fls disk.img -o 206848 3919
fls disk.img -o 206848 3916

icat disk.img -o 206848 2345 > key_file

chmod 600 key_file
ls
cat key_file
ssh -i key_file -p 50277 ctf-player@saturn.picoctf.net
	cat flag.txt
	
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{1k3y_513u7h_b5066e83f}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=PVeV-S3Zbqk&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=32


