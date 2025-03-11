
#### Description
Find the flag in the Python script![Download Python script](https://artifacts.picoctf.net/c/37/serpentine.py)

#### Hints 
1. Try running the script and see what happens
2. In the webshell, try examining the script with a text editor like `nano`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.
#### Solución:

1. Cambié el código usando nano, para que en la opción b me muestre la bandera.

````
    elif choice == 'b':
     # print('\nOops! I must have misplaced the print_flag function! Check my source code!\n\n')
     print_flag()




What would you like to do? (a/b/c) b
picoCTF{7h3_r04d_l355_7r4v3l3d_8e47d128}
a) Print encouragement
b) Print flag
c) Quit
`````

2.

````

`````


#### Pico:
picoCTF{7h3_r04d_l355_7r4v3l3d_8e47d128}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=sD-1ct_a8bc


