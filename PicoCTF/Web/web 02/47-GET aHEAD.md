
#### Description
Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:53554/](http://mercury.picoctf.net:53554/)

#### Hints 
1. Maybe you have more than 2 choices
2. Check out tools like Burpsuite to modify your requests and look at the responses



#### Solución:

1. Usamos el navegador Fire Fox:

````
Nos metimos al navegador y a la página, inspeccionamos y fuimos a la sección de red, luego hicimos un new request, pero en lugar de post usamos Head.
`````

![[Pasted image 20250322102038.png]]



2. La segunda opción es usar el comando Curl

````
Si se usa curl
`````
![[Pasted image 20250322113117.png]]



3. Usando la herramienta Burpsuite para usar un proxy:
![[Pasted image 20250322162823.png]]



#### Pico:
picoCTF{r3j3ct_th3_du4l1ty_2e5ba39f}


#### Notas adicionales:
Podemos usar Mozila para entender partes de web

Gráficamente podemos: Inspeccionas o ver el código fuente.
curl -I es equivalente a un método Head.

Hay varios métodos HTTP Request:
Get = curl - X GET www... :
Post = curl -X POST www...: Como para mandar credenciales
Put:
Delete:
Head = curl -I:
Patch:



Web Hacking Proxy: Es ponernos en medio e interceptar la comunicación, para poder hacer alteraciones.
#### Referencias:



