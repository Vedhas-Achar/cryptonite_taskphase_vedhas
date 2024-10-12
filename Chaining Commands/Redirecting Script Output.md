# Redirecting Script Output 

## Procedure
I started the challenge and then connected my terminal<br>
then i created `touch out.sh` and then appended using `echo /challenge/pwn >> out.sh` 
and `echo /challenge/college >> out.sh ` and then used `bash out.sh | /challenge/solve` 
to get my answer, and got the flag.

## bash
`hacker@chaining~redirecting-script-output:~$ touch out.sh
hacker@chaining~redirecting-script-output:~$ echo /challenge/pwn >> out.sh
hacker@chaining~redirecting-script-output:~$ echo /challenge/college >> out.sh
hacker@chaining~redirecting-script-output:~$ bash out.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{0BPaefqm6WiIEhF9_PmaqEWJ3O-.dhTM5QDLyIDO0czW}`

## Reference
Didnt use
