# Duplicating piped data with tee

## Procedure
i started the challenge and connected my terminal.<br>
then i used `/challenge/pwn | tee out` to get the output into an `out` file.
then used `cat out` to read the it and got the secret argument which i then used 
`/challenge/pwn --secret gle5uv8_ | /challenge/college` to get the flag.
i pasted that into the the flag box.

## bash
`Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee out
Processing...
You are trying to use 'tee' *instead* of /challenge/college. Use it *between*
/challenge/pwn and /challenge/college!
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ cat out
Usage: /challenge/pwn --secret [SECRET_ARG]
SECRET_ARG should be "gle5uv8_"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret gle
5uv8_ | tee /challenge/college
Processing...
You are trying to use 'tee' *instead* of /challenge/college. Use it *between*
/challenge/pwn and /challenge/college!
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret gle5uv8_ | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{gle5uv8_VnltUgF7LIPsz1tFaVR.dFjM5QDLyIDO0czW}`

## Reference
Real life friends.
