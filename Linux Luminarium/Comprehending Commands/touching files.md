# touching files

## Procedure
I started the challenge. and then connected the terminal.<br>
after that i used `pwd` and found that i was in `/hacker/a` hence i went back to `/` directory and then went into `/tmp` and used touch to make `pwn and college` and then went to `/` directory 
and then used `/challenge/run` to get my flag.

## bash
`Connected!
hacker@commands~touching-files:~$ LS
ssh-entrypoint: LS: command not found
hacker@commands~touching-files:~$ ls
a
hacker@commands~touching-files:~$ cd ../
hacker@commands~touching-files:/home$ cd ../
hacker@commands~touching-files:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~touching-files:/$ cd tmp
hacker@commands~touching-files:/tmp$ touch pwn college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.XvrUsDZh8M
hacker@commands~touching-files:/tmp$ cd ../
hacker@commands~touching-files:/$ /challenge/run
Success! Here is your flag:
pwn.college{kaz0DNdkj8-aK6l3xIKJ2_woNYw.dBzM4QDLyIDO0czW}`

## Reference
Didnt use
