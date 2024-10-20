# searching For Manuals

## Procedure
i started the challenge, and then connected my terminal. <br>
then i used `man man` and got the the manual of man, there i found something called `-K`
which is a brute force method to find something. i used that to get the challenge 
argument which gives me the flag, i used that to get the flag.
i pasted the flag in the flag box.

## bash
`Connected!
hacker@man~searching-for-manuals:~$ man -K pwn.college

CHALLENGE(1)                Challenge Commands                CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --sehztb NUM
              print the flag if NUM is 286

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-
       luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                      May 2024                     CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --sehztb 286
Correct usage! Your flag: pwn.college{s-2ehztEb8d6OkcyAFeqX60LPfb.dZTM4QDLyIDO0czW}`

## Reference
Didnt use
