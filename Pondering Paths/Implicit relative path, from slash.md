# Implicit relative path, from /

## Procedure
Start the clallenge, then i connected to my ubuntu terminal. then to find which path i am in, i used `pwd` after that i wanted to go to prev directoriees hence i used `cd ../`
after i reached the `/` directory i had lots of confusion and then got to know to run `challenge/run` and then found the flag which i copied to my Flag box.

## bash
`Connected!
hacker@paths~implicit-relative-paths-from-:~$ pwd
/home/hacker
hacker@paths~implicit-relative-paths-from-:~$ cd ../
hacker@paths~implicit-relative-paths-from-:/home$ cd ../
hacker@paths~implicit-relative-paths-from-:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{MgtpdrMdPR__1FV8PXg1yZ7QonX.dlDN1QDLyIDO0czW}`

## Reference
Google , Friends
