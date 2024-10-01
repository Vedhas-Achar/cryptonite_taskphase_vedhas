# Explicit relative path, from /

## Procedure
Start the clallenge, then i connected to my ubuntu terminal. then to find which path i am in, i used pwd after that i wanted to go to prev directoriees hence i used cd ../ after i reached the / directory i had lots of confusion and then got to know to do `./challenge/run` and then found the flag which i copied to my Flag box.

## bash
`Connected!
hacker@paths~explicit-relative-paths-from-:~$ pwd
/home/hacker
hacker@paths~explicit-relative-paths-from-:~$ ls
hacker@paths~explicit-relative-paths-from-:~$ cd /challenge
hacker@paths~explicit-relative-paths-from-:/challenge$ ./run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:/challenge$ cd ..
hacker@paths~explicit-relative-paths-from-:/$ cd ..
hacker@paths~explicit-relative-paths-from-:/$ pwd
/
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Q7xB3enOWESBWvH-yEc25CL7quM.dBTN1QDLyIDO0czW}`

## Reference
Group
