# Linking files

## Procedure
i started the program, and then connected the terminal<br>
after that i linked `ln -s /flag /home/hacker/not-the-flag` , and then i ran the program `/challenge/catflag`.
and got the flag, after that i pasted it and got it correct.
PS. (i made a mistake or removing the file and messing up stuff, but with the guidance of my mentor and got the answer)

## bash
`Connected!
hacker@commands~linking-files:~$ ls
a  flag  not-the-flag
hacker@commands~linking-files:~$ rm ./not-the-flag
hacker@commands~linking-files:~$ ls
a  flag
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{8mgIti21eEVqV7Nfk7pxWrnO5zJ.dlTM1UDLyIDO0czW}`

## Reference
mentor, friends, google
