
#### Description
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/4f3df7052b4121aff89af1a3f517afb1/dds1-alpine.flag.img.gz)

#### Hints 
1. Have you ever used `file` to determine what a file was?
2. Relevant terminal-fu in picoGym: https://play.picoctf.org/practice/challenge/85
3. Mastering this terminal-fu would enable you to find the flag in a single command: https://play.picoctf.org/practice/challenge/48
4. Using your own computer, you could use qemu to boot from this disk!


#### Solución:

#### 1. Usamos Slouth Kit 

````
1. Descargamos el archivo
2. Lo descomprimimos
	1. Es un archivo de imagen de disoc, almacena copia exacta de cualquier medio de almacenamiento
3. Una vez descomprimido usamos
	1. "srch_strings dds1-alpine.flag.img | grep pico"
4. Obtenemos la bandera
`````



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{for3ns1c4t0r_n30phyt3_a011c142}

#### Notas adicionales:
- Sleuth Kit, es para invesitgaciones forences
	- mmls
	- fls
	- icat
	- fsstat
	- blkakc
	-

Buscamos información en imágene de disco sin montar el disco

#### Referencias:
En clase


