# Executable shell script

## Procedure
I started the challenge and then connected my terminal<br>
then i used `touch script.sh ` to make the script, then i appended
`echo /challenge/solve >> script.sh` and then checked its permission,
changed its permission using `chmod a=rwx ./script.sh` and then ran it
using `./script.sh` and got my flag.

## bash
`Connected!
hacker@chaining~executable-shell-scripts:~$ touch script.sh
hacker@chaining~executable-shell-scripts:~$ echo /challenge/solve >> script.sh
hacker@chaining~executable-shell-scripts:~$ ls -l ./script.sh
-rw-r--r-- 1 hacker hacker 17 Oct 12 18:42 ./script.sh
hacker@chaining~executable-shell-scripts:~$ chmod o=rwx ./script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
ssh-entrypoint: ./script.sh: Permission denied
hacker@chaining~executable-shell-scripts:~$ chmod a=rwx ./script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{0V90tU4hUAfaxSCfLEHW0iFm-NR.dRzNyUDLyIDO0czW}`

## Reference
Didnt use
