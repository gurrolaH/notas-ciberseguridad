
#### Description
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with `nc jupiter.challenges.picoctf.org 15130`.



#### Hints 
1. I hear python can convert things.
2. It might help to have multiple windows open.


#### Solución:

1.- Use Cyberchef:

````
HBG-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 15130
Let us see how data is stored
colorado
Please give the 01100011 01101111 01101100 01101111 01110010 01100001 01100100 01101111 as a word.
...
you have 45 seconds.....

Input:
colorado
Please give me the  143 157 154 157 162 141 144 157 as a word.
Input:
colorado
Please give me the 636f6e7461696e6572 as a word.
Input:
container
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_02167de8}

------


Input: 01100011 01101111 01101100 01101111 01110010 01100001 01100100 01101111
	143 157 154 157 162 141 144 157
	636f6e7461696e6572

Recipe: From Octal, From Hex

Output: colorado, container

`````

2.

````

`````

#### Notas adicionales:
También se podía con Python. 
Podemos hay ocasiones que ya nos da la respuesta sin tener que ir a convertir la base.

#### Referencias:
https://gchq.github.io/CyberChef/#recipe=From_Octal('Space')&input=MTQzIDE1NyAxNTQgMTU3IDE2MiAxNDEgMTQ0IDE1Nw&ieol=CRLF&oeol=CRLF


https://gchq.github.io/CyberChef/#recipe=From_Hex('Auto')&input=NjM2ZjZlNzQ2MTY5NmU2NTcy&ieol=CRLF&oeol=CRLF



