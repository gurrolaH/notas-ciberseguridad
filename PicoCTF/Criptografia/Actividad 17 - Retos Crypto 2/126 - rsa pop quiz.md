
#### Description
Class, take your seats! It's PRIME-time for a quiz... `nc jupiter.challenges.picoctf.org 1981`

#### Hints 
1. [RSA info](https://simple.wikipedia.org/wiki/RSA_algorithm)


#### Solución:

#### 1. Usamos RSA

````
RSA - llave publica - asimetrico
-------------------------------------------------------------------------
m   - mensaje original o mensaje en texto plano 
c   - mensaje cifrado (ciphertext)
p,q - son dos numeros primos distintos y muy grandes
n   - es el modulo (lo compartes las llaves publica como privada)
tn  - totient n (funcion de euler)
e   - llave public - 65537 (exponente)  2 ^ 16 + 1
d   - llave privada

Calculos
--------------------------------------------------
n  = p * q
tn = (p -1) * (q-1)   ---> O
d = e ^ -1 (mod tn)	- pow(e, -1, tn)

Cifrar  
--------------------------------------------------
c = m ^ e (mod n)	- pow(m, e, n)

Decifrars
--------------------------------------------------
m = c ^ d (mod n)	- pow(c, d, n)



Cifrar y Descifrar se relacionan de forma matemática.
Números primos grandes son más seguros



-------------------------------------------------
Lo hice en Windows para ello usé
- pip install pwntools


------------------------------------------------
Usé el exp.py del profe, pero no me funcionó, por lo que una IA me recomendó a partir del punto 8, cambiar a lo siguiente:

#8

print(r.recvuntil(b'):').decode())

r.sendline(b'Y')

print(r.recvuntil(b': ').decode())

  

p = 153143042272527868798412612417204434156935146874282990942386694020462861918068684561281763577034706600608387699148071015194725533394126069826857182428660427818277378724977554365910231524827258160904493774748749088477328204812171935987088715261127321911849092207070653272176072509933245978935455542420691737433

c = 18031488536864379496089550017272599246134435121343229164236671388038630752847645738968455413067773166115234039247540029174331743781203512108626594601293283737392240326020888417252388602914051828980913478927759934805755030493894728974208520271926698905550119698686762813722190657005740866343113838228101687566611695952746931293926696289378849403873881699852860519784750763227733530168282209363348322874740823803639617797763626570478847423136936562441423318948695084910283653593619962163665200322516949205854709192890808315604698217238383629613355109164122397545332736734824591444665706810731112586202816816647839648399

e = 65537

n = 23952937352643527451379227516428377705004894508566304313177880191662177061878993798938496818120987817049538365206671401938265663712351239785237507341311858383628932183083145614696585411921662992078376103990806989257289472590902167457302888198293135333083734504191910953238278860923153746261500759411620299864395158783509535039259714359526738924736952759753503357614939203434092075676169179112452620687731670534906069845965633455748606649062394293289967059348143206600765820021392608270528856238306849191113241355842396325210132358046616312901337987464473799040762271876389031455051640937681745409057246190498795697239

# Verificar que p es factor de n

assert n % p == 0, "p no es un factor primo de n"


# Calcular q y φ(n)

q = n // p

phi = (p - 1) * (q - 1)

  
# Calcular d (clave privada)

d = pow(e, -1, phi)

# Descifrar

m = pow(c, d, n)

# Enviar el resultado (en decimal)

print('m=' + str(m))

r.sendline(str(m).encode())

-- Creo solo cambia lo de ASSERT
`````




--- 
---
#### 2.

````

`````


#### Pico:
picoCTF{wA8_th4t$_ill3aGal..ode01e4bb}

#### Notas adicionales:


#### Referencias:
Clase y https://drive.google.com/file/d/1SYaXmLOP8z28r5LhsZMlMFzpggo-upEO/view



