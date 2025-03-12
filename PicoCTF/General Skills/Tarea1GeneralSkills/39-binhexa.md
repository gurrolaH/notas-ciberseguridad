
#### Description
How well can you perfom basic binary operations?Start searching for the flag here `nc titan.picoctf.net 62744`

#### Hints 
None

#### Solución:

1. Usamos operaciones para números binarios con una calculadora.

````
HBG-picoctf@webshell:~$ nc titan.picoctf.net 62744

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 11011101
Binary Number 2: 11011110


Question 1/6:
Operation 1: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 110111010
Correct!

Question 2/6:
Operation 2: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 11011.11

Incorrect input. Provide the right input
Enter the binary result: 1101111
Correct!

Question 3/6:
Operation 3: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 1011111110100110
Correct!

Question 4/6:
Operation 4: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11011111
Correct!

Question 5/6:
Operation 5: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 110111011
Correct!

Question 6/6:
Operation 6: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11011100
Correct!

Enter the results of the last operation in hexadecimal: 16
Incorrect answer!

Enter the results of the last operation in hexadecimal: DC

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_1367e2c6}
`````

2.

````

`````


#### Pico:
picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_1367e2c6}

#### Notas adicionales:
Esta página tiene una buena calculadora para número binarios:
https://www.rapidtables.com/calc/math/binary-calculator.html


#### Referencias:
https://www.youtube.com/watch?v=uWJbfL4o4Nk

https://www.rapidtables.com/calc/math/binary-calculator.html?num1=11011101&op=5&num2=11011110

