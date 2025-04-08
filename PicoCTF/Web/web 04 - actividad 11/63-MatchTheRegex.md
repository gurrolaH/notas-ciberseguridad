
#### Description
How about trying to match a regular expression

Additional details will be available after launching your challenge instance.

How about trying to match a regular expressionThe website is running [here](http://saturn.picoctf.net:56316/).
#### Hints 
1. Access the webpage and try to match the regular expression associated with the text field


#### Solución:

1. Usamos expresiones regulares:

````
- Supimos que se tenía que validar una expresión regular, por el html.
- Nos fuimos a regexr.com para saber que es lo que validaría.
- Le pegamos la expresión que había en el código.
`````
![[Pasted image 20250407072659.png]]
![[Pasted image 20250407072549.png]]
2.

````

`````


#### Pico:
`picoCTF{succ3ssfully_matchtheregex_f89ea585}`


#### Notas adicionales:
No debemos hacer validaciones con expresiones regulares, y menos en el código de html, ya que hay forma de encontrar las validaciones.

#### Referencias:
https://regexr.com/


