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
