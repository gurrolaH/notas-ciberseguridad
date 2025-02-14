
#### Description

Can you convert the number 42 (base 10) to binary (base 2)?


#### Hints 

Submit your answer in our competition's flag format. For example, if your answer was '11111', you would submit 'picoCTF{11111}' as the flag.

## Solución 
Python:
````
HBG-picoctf@webshell:~$ python
Python 3.10.12 (main, Sep 11 2024, 15:47:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> bin(42)
'0b101010'
>>> bin(42)[2:]
'101010'
```
````

1. Cyberchef
````
En el input: 40
Recipes:
From Decimal
To Binary:

Output:
00101010
````

## Referencias
https://gchq.github.io/CyberChef/#recipe=From_Decimal('Space',false)To_Binary('Space',8)&input=NDI