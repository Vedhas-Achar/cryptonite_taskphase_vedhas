# Learning From Documentation

## Procedure
I started the challenge, i connected it to my terminal. <br>
then i used `pwd` to get to know my location, after that i traversed to `/challenge` to 
check if theres another `challenge` file, when i comfirmed that, i used `/challenge/challenge
 --giveflag`. and then pasted the flag into the box.

## bash
`Connected!
hacker@man~learning-from-documentation:~$ ls
a  flag  not-the-flag
hacker@man~learning-from-documentation:~$ cd ..
hacker@man~learning-from-documentation:/home$ cd ..
hacker@man~learning-from-documentation:/$ cd challenge
hacker@man~learning-from-documentation:/challenge$ ls
DESCRIPTION.md  challenge
hacker@man~learning-from-documentation:/challenge$ cd
hacker@man~learning-from-documentation:~$ ~/challenge --giveflag
ssh-entrypoint: /home/hacker/challenge: No such file or directory
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{sVsLQNv9Uw62RyQPRB5YzLip9S6.dRjM5QDLyIDO0czW}`

## Reference
Didnt use
