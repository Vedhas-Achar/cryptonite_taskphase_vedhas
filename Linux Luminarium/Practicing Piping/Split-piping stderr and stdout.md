# Split-piping stderr and stdout

## Procedure
i started the challenge and then connected the terminal<br>
then i use i try errors lots of ways but then didnt get it, hence i copiloted it.
i got to know that we had to use `> >` way, hence i did that on my own by typing
`/challenge/hack > >(/challenge/planet) 2> >(/challenge/the)` and got the flag
which i then pasted into the flag box.

## bash
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | tee >(/challenge/planet) 2>(/challenge/the)
tee: 2/dev/fd/62: No such file or directory
This secret data must directly make it to /challenge/planet over my stdout.
Don't try to copy-paste it; it changes too fast.
998522197121196559
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | 2>(/challenge/the) >(/challenge/planet)
ssh-entrypoint: 2/dev/fd/63: No such file or directory
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | 2>&1(/chal
lenge/the) >(/challenge/planet)
ssh-entrypoint: syntax error near unexpected token '('
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | 2>&1 /chal
lenge/the >(/challenge/planet)
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challen
ge/planet) > 2> (/challenge/the)
ssh-entrypoint: syntax error near unexpected token 2
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> > (/challenge/the)
ssh-entrypoint: syntax error near unexpected token >
`hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{Uk6zSYGiTMmV7FYwx4I3EPQ-0wa.dFDNwYDLyIDO0czW}`

## Reference
Copilot
