# Changing permission

## Procedure
I started the challenge and then terminal<br>
then i used `ls -l /flag` to get to know my permissions, then i used `chmod o+r` to
give myself reading permission, then i used `cat /flag ` to get the flag

## bash
`hacker@permissions~changing-permissions:~$ ls -l /flag
-r--r----- 1 root root 58 Oct 11 08:02 /flag
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{kEpD0QRLHOX1QXaJkZjhxBrXjgg.dNzNyUDLyIDO0czW}`

## Reference
Didnt use
