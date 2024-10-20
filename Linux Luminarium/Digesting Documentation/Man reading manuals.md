## Man reading manuals

## Procedure
i started the challenge, and then connected my terminal. <br>
after that i used `man challenge` and got description of challenge, after that it said to used `/challenge/challenge --dobxya 814`, and then got the flag.<br>
i pasted the flag to the box.

## bash
`Connected!
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

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

       --dobxya NUM
              print the flag if NUM is 814

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)
hacker@man~reading-manuals:~$ /challenge/challenge --dobxya 814
Correct usage! Your flag: pwn.college{AZIDXd81OobxRyaQ-OjdrmJPQEa.dRTM4QDLyIDO0czW}`

## Reference
Didnt use
