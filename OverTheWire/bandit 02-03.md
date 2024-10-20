# bandit 2-3

## Procedure
I started the challenge<br>
then i used `ls` to find the file, then i used `cat "spaces in this filename"` and 
got the password.

## bash
`bandit2@bandit:~$ cd
bandit2@bandit:~$ cat ./"spaces in this filename
cat: './spaces in this filename'$'\n': No such file or directory
bandit2@bandit:~$ cd
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat "spaces in this filename"
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx`

## Reference
Didnt use
