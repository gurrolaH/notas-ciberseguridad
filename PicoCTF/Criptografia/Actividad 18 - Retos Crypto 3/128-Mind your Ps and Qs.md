
#### Description
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values)

#### Hints 
1. Bits are expensive, I used only a little bit over 100 to save money


#### Solución:

#### 1. Usamos descifrado para RSA

````
Usamos la página de: "dcode RSA, rsa cipher"

Usamos los valores, que descargamos del reto;

Esto que tiene asteriscos me lo dio deepseek-------------
- **C** = Mensaje cifrado
    
- **E** = Exponente público (típico 65537)
    
- **N** = Módulo público (producto de dos primos grandes)
-----------------------------------------------------------
c: 861270243527190895777142537838333832920579264010533029282104230006461420086153423

n: 1311097532562595991877980619849724606784164430105441327897358800116889057763413423

e: 65537

`````
![[Pasted image 20250521234420.png]]



--- 
---
#### 2.

````

`````




#### Pico:
picoCTF{sma11_N_n0_g0od_13686679}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=pdAHWr5cxRc


