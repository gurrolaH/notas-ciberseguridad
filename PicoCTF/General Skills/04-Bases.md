#### Description

What does this `bDNhcm5fdGgzX3IwcDM1` mean? I think it has something to do with bases.

#### Hints 


Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{hello}' as the flag.

## Soluciones:
Cyberchef

````
Input:bDNhcm5fdGgzX3IwcDM1
Recipe: From Base64
Output: l3arn_th3_r0p35
`````

Python:
````
>>> python
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'python' is not defined
>>> import base64
>>> base64.b64decode('bDNhcm5fdGgzX3IwcDM1')
b'l3arn_th3_r0p35'

`````


picoCTF(l3arn_th3_r0p35)


Notas adicionales:

## Referencias:
https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true,false)&input=YkROaGNtNWZkR2d6WDNJd2NETTEK

