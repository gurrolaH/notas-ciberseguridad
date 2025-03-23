
#### Description
This website can be rendered only by **picobrowser**, go and catch the flag! `https://jupiter.challenges.picoctf.org/problem/50522/` ([link](https://jupiter.challenges.picoctf.org/problem/50522/)) or http://jupiter.challenges.picoctf.org:50522

#### Hints 
1. You don't need to download a new web browser


#### Solución:

1. Cambiamos algunas propiedades en User Agent.

````
HBG-picoctf@webshell:~$ curl -s https://jupiter.challenges.picoctf.org/problem/50522/flag -H "User-Agent: picobrowser" | grep pico
         <!-- <strong>Title</strong> --> picobrowser!
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{p1c0_s3cr3t_ag3nt_51414fa7}</code></p>
`````

2. Se puede hacer desde el mismo navegador, pero solo en fire fox, en Chrome no.

````

`````


#### Pico:
picoCTF{p1c0_s3cr3t_ag3nt_51414fa7}


#### Notas adicionales:


#### Referencias:



