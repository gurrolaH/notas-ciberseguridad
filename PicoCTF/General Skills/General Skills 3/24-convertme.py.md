
#### Description
Run the Python script and convert the given number from decimal to binary to get the flag.[Download Python script](https://artifacts.picoctf.net/c/22/convertme.py)

#### Hints 
1. Look up a decimal to binary number conversion app on the web or use your computer's calculator!
2. The `str_xor` function does not need to be reverse engineered for this challenge.
3. If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
4. If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
5. Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
6. Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 convertme.py`

#### Solución:

1. Usamos la función bin() de mismo python para decifrar la password y entrar a ver la bandera.

````
┌──(kali㉿kali)-[/home/kali]
└─PS> python3 ./convertme.py                                                                                                                                    
If 86 is in decimal base, what is it in binary base?
Answer: 1010110
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_762f748e}
                                                                                                                           

┌──(kali㉿kali)-[/home/kali]
└─PS> picoCTF{4ll_y0ur_b4535_762f748e}
`````

2.

````

`````


#### Pico:
picoCTF{4ll_y0ur_b4535_762f748e}

#### Notas adicionales:
Use python dentro de la misma consola de linux.

#### Referencias:
Use python


