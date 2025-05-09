cl
#### Description
Download the disk image and use `mmls` on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.[Download disk image](https://artifacts.picoctf.net/c/164/disk.img.gz)

Additional details will be available after launching your challenge instance.

#### Hints 
(None)


#### Solución:

#### 1. Usamos comando de Slouth Kit
![[Pasted image 20250508170252.png]]

````
wget "https://artifacts.picoctf.net/c/164/disk.img.gz"
sl
ls
gzip -d disk.img.gz
ls
ls -lah disk.img
mmls disk.img
	- Obtuvimos el Length para Linux
nc saturn.picoctf.net 50398
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{mm15_ftw!}

#### Notas adicionales:
- mmls nos ayuda a saber tamaños y posiciones de las particiones.

#### Referencias:
Comandos vistos en la clase


