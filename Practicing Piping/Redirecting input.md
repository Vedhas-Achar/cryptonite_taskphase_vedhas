# Redirecting input 

## Procedure
I started the challenge, then connected my terminal<br>
then i used `echo COLLEGE > PWN` and added the `COLLEGE` into the `PWN` file,
then i used `< PWN /challenge/run` and then got the flag which i pasted into 
the flag box.

## bash
`Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challege/run < PWN
ssh-entrypoint: /challege/run: No such file or directory
hacker@piping~redirecting-input:~$ pwd
/home/hacker
hacker@piping~redirecting-input:~$ PWN < /challenge/run
ssh-entrypoint: PWN: command not found
hacker@piping~redirecting-input:~$ cat PWN
COLLEGE
hacker@piping~redirecting-input:~$ echo PWM > /challenge/run
ssh-entrypoint: /challenge/run: Permission denied
hacker@piping~redirecting-input:~$ < PWN /challenge/run
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{0oMGv1lfUG8KkyljpidzlWPTW1e.dBzN1QDLyIDO0czW}`

## Reference
Didnt use
