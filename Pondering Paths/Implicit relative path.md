# Implicit relative path

## Procedure
Start the clallenge, then i connected to my ubuntu terminal. then to find which path i am in, i used pwd after that i wanted to go to prev directoriees hence 
i used cd ../ after i reached the / directory. Then i went into challenge folder and then typed `./run`, and then found the flag which i copied to my Flag box.

## bash
`Connected!
hacker@paths~implicit-relative-path:~$ pwd
/home/hacker
hacker@paths~implicit-relative-path:~$ cd ..
hacker@paths~implicit-relative-path:/home$ cd ..
hacker@paths~implicit-relative-path:/$ pwd
/
hacker@paths~implicit-relative-path:/$ cd challenge
hacker@paths~implicit-relative-path:/challenge$ ls
DESCRIPTION.md  run
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Ux0_A7qKn1YbQ5cPVbybw053Wuo.dFTN1QDLyIDO0czW}`

## Reference
Didnt use
