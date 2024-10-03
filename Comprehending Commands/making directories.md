# making directories

## Procedure
I started the challenge, connected my terminal. <br>
then i found that i was in `/home/hacker` hence i went back to `/` directory. and then 
and then went into `/tmp` and then used `mkdir pwn` to create `pwn`, and then used
`touch college` to make the file. then used `/challenge/run` to get the flag.

## bash 
`Connected!
hacker@commands~making-directories:~$ pwd
/home/hacker
hacker@commands~making-directories:~$ cd ..
hacker@commands~making-directories:/home$ cd ..
hacker@commands~making-directories:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~making-directories:/$ cd /tmp
hacker@commands~making-directories:/tmp$ ls
bin  hsperfdata_root  tmp.XvrUsDZh8M
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.XvrUsDZh8M
hacker@commands~making-directories:/tmp$ cd pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{s7nBkEn2cY7tFhLBNnsV3A78qyC.dFzM4QDLyIDO0czW}`

## Reference
Didnt use
