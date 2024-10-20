# Changing file ownership

## Procedure
I started the challenge and then connected my terminal<br>
then i used `ls -l` to see the files, then i used `chown hacker not-the-flag`
and then read the flag using `cat /flag` and then got the flag which i then pasted into the 
box.

## bash
`Connected!
hacker@permissions~changing-file-ownership:~$ ls -l
total 36
-rw-r--r-- 1 hacker hacker   4 Oct  8 04:57 COLLEGE
-rw-r--r-- 1 hacker hacker   8 Oct  8 17:24 PWN
-rw-r--r-- 1 root   hacker  58 Oct  2 17:53 a
-rw-r--r-- 1 root   root    58 Oct  4 12:11 flag
-rw-r--r-- 1 hacker hacker 829 Oct  8 05:29 instructions
-rw-r--r-- 1 hacker hacker  22 Oct  8 05:07 myfile
-rw-r--r-- 1 hacker hacker  93 Oct  8 05:29 myflag
lrwxrwxrwx 1 hacker hacker   5 Oct  5 15:23 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker  77 Oct  8 18:56 out
-rw-r--r-- 1 hacker hacker 435 Oct  8 05:15 the-flag
hacker@permissions~changing-file-ownership:~$ chown hacker not-the-flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{8CFx5plWcDD33xZjWNUjTnFQ8Tn.dFTM2QDLyIDO0czW}`

## Reference
Didnt use
