
#### Description
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/70/challenge.zip)

#### Hints 
1. `git branch -a` will let you see available branches
2. How can file 'diffs' be brought to the main branch? Don't forget to `git config`!
3. Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim


#### Solución:

1. Básicamente lo que hicimos fue estar mezclando las diferentes ramas que había, solucionando igual los problemas que hubiera.

  feature/part-1
  feature/part-2
  feature/part-3

````
HBG-picoctf@webshell:~$ cd drop-in/
HBG-picoctf@webshell:~/drop-in$ git branch -a

[1]+  Stopped                 git branch -a
HBG-picoctf@webshell:~/drop-in$ git merge feature/part-1
Updating 54c7842..f65544e
Fast-forward
 flag.py | 1 +
 1 file changed, 1 insertion(+)
HBG-picoctf@webshell:~/drop-in$ ls      
flag.py
HBG-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')HBG-picoctf@webshell:~/drop-in$ git merge feature/part-2
Committer identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'HBG-picoctf@webshell.(none)')
HBG-picoctf@webshell:~/drop-in$   git config --global user.email "you@example.com"
HBG-picoctf@webshell:~/drop-in$   git config --global user.name "Your Name"
HBG-picoctf@webshell:~/drop-in$ git merge feature/part-2
Auto-merging flag.py
CONFLICT (content): Merge conflict in flag.py
Automatic merge failed; fix conflicts and then commit the result.
HBG-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")
<<<<<<< HEAD
print("picoCTF{t3@mw0rk_", end='')
=======

print("m@k3s_th3_dr3@m_", end='')
>>>>>>> feature/part-2
HBG-picoctf@webshell:~/drop-in$ git merge eature/part-3
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
HBG-picoctf@webshell:~/drop-in$ git merge feature/part-3
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
HBG-picoctf@webshell:~/drop-in$ git add flag.py 
HBG-picoctf@webshell:~/drop-in$ git commit -m merge1
[main 0fa200a] merge1
HBG-picoctf@webshell:~/drop-in$ git merge feature/part-3
Auto-merging flag.py
CONFLICT (content): Merge conflict in flag.py
Automatic merge failed; fix conflicts and then commit the result.
HBG-picoctf@webshell:~/drop-in$ git add flag.py 
HBG-picoctf@webshell:~/drop-in$ git commit -m merge2
[main cfb5f4e] merge2
HBG-picoctf@webshell:~/drop-in$ cat flag.py 
print("Printing the flag...")
<<<<<<< HEAD
<<<<<<< HEAD
print("picoCTF{t3@mw0rk_", end='')
=======

print("m@k3s_th3_dr3@m_", end='')
>>>>>>> feature/part-2
=======

print("w0rk_7ffa0077}")
>>>>>>> feature/part-3
`````

2.

````

`````


#### Pico:
picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}

#### Notas adicionales:


#### Referencias:
https://www.youtube.com/watch?v=_CH5IQewkzw



