
#### Description
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/18/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/18/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/18/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

#### Hints 
1. To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
2. To exit `bvi` type `:q` and press enter.
3. The `str_xor` function does not need to be reverse engineered for this challenge.


#### Solución:

1. Vi un video para solucionar este ejercicios, básicamente lo que hace es modificar el código de py para que imprima las contraseñas posibles en un bucle y las vaya probando.

````
# The strings below are 7 possibilities for the correct password.

#   (Only 1 is correct)

pos_pw_list = ["8799", "d3ab", "1ea2", "acaf", "2295", "a9de", "6f3d"]

  
  

def level_3_pw_check():

    #user_pw = input("Please enter correct password for flag: ")

    for user_pw in pos_pw_list:

        user_pw_hash = hash_pw(user_pw)

  
        if( user_pw_hash == correct_pw_hash ):

            print("Welcome back... your flag, user:")

            decryption = str_xor(flag_enc.decode(), user_pw)

            print(decryption)

            print("Contrasenia: " + user_pw)

            return

        print("That password is incorrect")
`````

2.

````

`````


#### Pico:
picoCTF{m45h_fl1ng1ng_6f98a49f}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=Dn4NruKchkw

