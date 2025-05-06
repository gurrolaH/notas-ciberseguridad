
#### Description
We found this [file](https://mercury.picoctf.net/static/06a5e4ab22ba52cd66a038d51a6cc07b/tunn3l_v1s10n). Recover the flag.

#### Hints 
1. Weird that it won't display right...

#### Solución:

#### 1. Se resolvió usando "hexeditor"
![[Pasted image 20250506080712.png]]

````
1. Se analizan los Magic Bytes
2. Se hace el archivo con la extensión que corresponda según el encabezado en hex
3. Se acomodan los Bytes según correspondan al archivo, para que sean correctos
4. Se amplía la imagen en lo alto, en este caso se hizo modificando los hexadecimales

Comandos usados:
- hexeditor
`````




--- 
---
#### 2.

````

`````


#### Pico:
![[Pasted image 20250506080649.png]]
picoCTF{qu1t3_a_v13w_2020}


#### Notas adicionales:
- Debemos cuidar que los encabezados estén correctamente según el tipo de archivo
- Se debe analizar las dimensiones de la imagen


#### Referencias:
https://www.youtube.com/watch?v=1ucy2G1PIh4&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=27


