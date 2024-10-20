# Helpful Programs

## Procedure
I started the challenge, and then connected my terminal<br>
after that i used `/challenge/challenge --help` and got the way of using it,
i had to first use `/challenge/challenge -p` to get the secret value,
i used `/challenge/challenge -g 486` and that gave me my flag.
i pasted the flag into flag box.

## bash 
`hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to
                        give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -g
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument
hacker@man~helpful-programs:~$ /challenge/challenge --give-the-flag
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument
hacker@man~helpful-programs:~$ /challenge/challenge -g GIVE_THE_FLAG
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: invalid int value: 'GIVE_THE_FLAG'
hacker@man~helpful-programs:~$ -p
ssh-entrypoint: -p: command not found
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 485
hacker@man~helpful-programs:~$ /challenge/challenge -g 485
Correct usage! Your flag: pwn.college{AZn4J8UwTn5KDX6pS-xfE9U9KDr.ddjM4QDLyIDO0czW}`

## Reference
Real Friends
