
#### Description
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/61864/` or http://jupiter.challenges.picoctf.org:61864


#### Hints 
1. What is that cookie?
2. Have you heard of JWT?


#### Solución:

1. Usamos herramientas para leer los JWT, luego editarlo, y con john de kali sacamos la clave para token.

````

`````
![[Pasted image 20250327212252.png]]
![[Pasted image 20250327212321.png]]

![[Pasted image 20250327213209.png]]

![[Pasted image 20250327214441.png]]




###### 2. La segunda opción era hacer una script para editar el token, desde la librería jwt en py.

````

`````

![[Pasted image 20250328105214.png]]



#### Pico:
picoCTF{jawt_was_just_what_you_thought_1ca14548}
![[Pasted image 20250328105315.png]]


#### Notas adicionales:


#### Referencias:



