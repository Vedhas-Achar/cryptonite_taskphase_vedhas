# Resuming Processes

## Procedure
i started the challenge and then connected the terminal<br>
and then used `/challenge/run` to get the process going, then i used `Ctrl-Z` to
suspend it which i then resumed using `fg /chalenge/run` and got the flag.

## bash
`Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg /challenge/run
/challenge/run
I'm back! Here's your flag:
pwn.college{QVbA4x1pCaix6MCHLft-_WzjlWk.dZDN4QDLyIDO0czW}`

## Reference
Didnt use
