
#### Description
I don't like scrolling down to read the code of my website, so I've squished it. As a bonus, my pages load faster!Browse [here](http://titan.picoctf.net:54386/), and find the flag!


#### Hints 
1. Try CTRL+U / ⌘+U in your browser to view the page source. You can also add 'view-source:' before the URL, or try `curl <URL>` in your shell.
2. Minification reduces the size of code, but does not change its functionality.
3. What tools do developers use when working on a website? Many text editors and browsers include formatting.


#### Solución:

1. Fuimos al código fuente.

````
- El código no se podía scrollear, pero había mucho texto comprimido en una sola línea, para que la página fuera más rápida.
- Use el ctrl + F para buscar el patrón picoCTF.
`````
![[Pasted image 20250405154830.png]]
2.

````

`````


#### Pico:
picoCTF{pr3tty_c0d3_dbe259ce}

#### Notas adicionales:
- Ni comprimiendo todo el texto en una sola línea es segura, hay que cuidar el código html.

#### Referencias:



