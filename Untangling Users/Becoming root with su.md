# Becoming Root with su

## Procedure
I started the challenge and then connected my terminal<br>
then i looked up `ls -l /flag` and then typed `su` to get root user.
then i used `chmod a+rwx /flag` to make the flag readable, then used `/flag` to get the flag.

## bash
`Connected!
hacker@users~becoming-root-with-su:~$ ls -l /flag
-r-------- 1 root root 58 Oct 12 12:50 /flag
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# /flag
bash: /flag: Permission denied
root@users~becoming-root-with-su:/home/hacker# chmod a+rmx /flag
chmod: invalid mode: ‘a+rmx’
Try 'chmod --help' for more information.
root@users~becoming-root-with-su:/home/hacker# chmod a+rwx /flag
root@users~becoming-root-with-su:/home/hacker# /flag
/flag: line 1: pwn.college{MobOXLcYCT_S0bKs9mKfmdYsOlW.dVTN0UDLyIDO0czW}`

## Reference
Didnt use
