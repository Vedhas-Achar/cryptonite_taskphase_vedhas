# Adding Commands

## Procedure
I started the challenge and then connected my terminal<br>
And then i tried lots of ways but didnt seem to get it to work, hence i asked copilot to help,
then i used `echo '#!/bin/bash' > win` and then used `echo 'cat /flag' >> ~/win` so that it runs 
`/flag` then i typed `chmod +x ~/win` to give executable to it, and then i used
`PATH=~/:$PATH` to append home directory to the path, then finally i used `/challenge/run` 
to get the flag.

## bash
`hacker@path~adding-commands:~$ echo '#!/bin/bash' >
ssh-entrypoint: syntax error near unexpected token newline'
hacker@path~adding-commands:~$ echo '#!/bin/bash' > win
hacker@path~adding-commands:~$ echo 'cat /flag' >> ~/win
hacker@path~adding-commands:~$ chmod +x ~/win
hacker@path~adding-commands:~$ PATH=~/:$PATH
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{UwgwHeWZn6aNnIYvp_yy_2ezJT6.dZzNyUDLyIDO0czW}`

## Reference
Copilot AI
