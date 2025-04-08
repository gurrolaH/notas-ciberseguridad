
#### Description
I found a web app that can help process images: PNG images only!

Additional details will be available after launching your challenge instance.

#### Hints 
None

#### Solución:

#### 1.

````
- Subimos un arhivo jugando con las extensiones para que fuera un png, pero en realidad era un php.
- Ajustamos para que burlara los metadatos de png.
- El archivo llevaba un php, que nos daba acceso web shell.
- Comenzamos a navegar desde el cmd en la URL.
- Encontramos la bandera en un archivo.
`````

![[Pasted image 20250407170745.png]]

![[Pasted image 20250407170724.png]]


![[Pasted image 20250407170948.png]]



--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_3f706222}

#### Notas adicionales:
Debemos cuidar que no se pueda ejecutar código php desde las páginas web, y esto se común cuando son páginas en las que se puede subir archivos.

#### Referencias:
https://www.youtube.com/watch?v=co8MZmviC1U


