# Fun with group names

## Procedure
i started the challenge and then connected my terminal<br>
then i checked my id, i was `grp13277` hence i used `ls -l` to see where the flag was.
then i changed its group using `chgrp grp13277 /flag` and then used `cat /flag` to 
get my flag.

## bash
`                                                                            Connected!
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp13277) groups=1000(grp13277)
hacker@permissions~fun-with-groups-names:~$ ls -l
total 36
-rw-r--r-- 1 hacker grp13277   4 Oct  8 04:57 COLLEGE
-rw-r--r-- 1 hacker grp13277   8 Oct  8 17:24 PWN
-rw-r--r-- 1 root   grp13277  58 Oct  2 17:53 a
-rw-r--r-- 1 root   grp13277  58 Oct  4 12:11 flag
-rw-r--r-- 1 hacker grp13277 829 Oct  8 05:29 instructions
-rw-r--r-- 1 hacker grp13277  22 Oct  8 05:07 myfile
-rw-r--r-- 1 hacker grp13277  93 Oct  8 05:29 myflag
lrwxrwxrwx 1 hacker grp13277   5 Oct  5 15:23 not-the-flag -> /flag
-rw-r--r-- 1 root   grp13277  77 Oct  8 18:56 out
-rw-r--r-- 1 hacker grp13277 435 Oct  8 05:15 the-flag
hacker@permissions~fun-with-groups-names:~$ chgrp grp13277 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{ggOnsoTbb02ExoFv6NwBiUg4MW7.dJzNyUDLyIDO0czW}`

## Reference
Didnt use
