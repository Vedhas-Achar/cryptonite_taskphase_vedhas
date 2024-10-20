# the SUID bit

## Procedure
I started the challenge and then connected my terminal<br>
and then i saw the permission of `/challengw/getroot` and then used
`chmod u+s /challenge/getroot` and then ran it , i went into SUID root,
then i used `chown root /flag` and then used `cat /flag` to got the flag.

## bash
`Connected!
hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwxr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat flag
pwn.college{EZ_d7zdmFqjaCRqB5o2qGsrGLN2.dFzN1QDLyIDO0czW}
root@permissions~the-suid-bit:~# ls
COLLEGE  a     instructions  myflag        out
PWN      flag  myfile        not-the-flag  the-flag
root@permissions~the-suid-bit:~# ls -l
total 36
-rw-r--r-- 1 hacker hacker   4 Oct  8 04:57 COLLEGE
-rw-r--r-- 1 hacker hacker   8 Oct  8 17:24 PWN
-rw-r--r-- 1 root   hacker  58 Oct  2 17:53 a
-rw-r--r-- 1 root   hacker  58 Oct  4 12:11 flag
-rw-r--r-- 1 hacker hacker 829 Oct  8 05:29 instructions
-rw-r--r-- 1 hacker hacker  22 Oct  8 05:07 myfile
-rw-r--r-- 1 hacker hacker  93 Oct  8 05:29 myflag
lrwxrwxrwx 1 hacker hacker   5 Oct  5 15:23 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker  77 Oct  8 18:56 out
-rw-r--r-- 1 hacker hacker 435 Oct  8 05:15 the-flag
root@permissions~the-suid-bit:~# id
uid=0(root) gid=1000(hacker) groups=1000(hacker)
root@permissions~the-suid-bit:~# chown root /flag
root@permissions~the-suid-bit:~# cat /flag
pwn.college{44eyMYEAT92s9r4nsIGmi_4Eov9.dNTM2QDLyIDO0czW}`

## Reference
Didnt use
