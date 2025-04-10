
#### Description
We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.

#### Hints 
1. Try fixing the file header


#### Solución:

#### 1. Acomodamos el mal formato que traía en metadatos

````
- Acomodamos el encabezado para que fuera un encabezado correcto, lo hicimos acomodando los hexadecimales.
- Corregimos el encabezado
- Corregimos los chunks.
- Instalamos pngcheck.
- Nos iba indicando que teníamos dañada una imágen y nos daba los errores
`````

Comandos Utilizados en el proceso:
![[Pasted image 20250409225703.png]]



--- 
---
#### 2.

````

`````


#### Pico:
![[Pasted image 20250409225033.png]]
picoCTF{corrupt10n_1847995}

#### Notas adicionales:
Se pueden dañar archivos cambiando los encabezados.
También si tiene mal los chunks.

#### Referencias:
https://www.youtube.com/watch?v=7zY4VkiWbBI


