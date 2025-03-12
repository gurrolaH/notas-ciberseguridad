#### Description
Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM)Start your instance to see connection details.`ssh -p 55953 ctf-player@saturn.picoctf.net`The password is `af86add3`


#### Hints 
1. Experiment with different shell syntax


#### Solución:

1. Lo vi en un video, pero no le entendí mucho la vaerdad de porqué usar esta línea: clear & find .

````
Special$ clear & find .
Clear & find . 
sh: 1: Clear: not found
.
./blargh
./blargh/flag.txt
./.cache
./.cache/motd.legal-displayed
Special$ clear & cat ./blargh/flag.txt
Clear & cat ./blargh/flag.txt 
sh: 1: Clear: not found
picoCTF{5p311ch3ck_15_7h3_w0r57_6a2763f6}Special$ Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.
`````

2.

````

`````


#### Pico:
picoCTF{5p311ch3ck_15_7h3_w0r57_6a2763f6}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=6lEd1yVsxpw


