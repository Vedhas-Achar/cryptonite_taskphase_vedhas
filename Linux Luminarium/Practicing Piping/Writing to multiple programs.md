# Writing to multiple programs

## Procedure
i started the challenge and then connected to my terminal<br>
then  i used `/challenge/hack | tee >/challenge/the >/challenge/planet` thinking it would 
world, but then it didnt work at all. after lots of thinking i gave up and asked copilot
for the answer.... copilot told to put brackets for the path, hence now i typed
`/challenge/hack | tee >(/challenge/the) >(/challenge/planet)` and it worked and got the flag.
which i pasted into the flag box.

## bash
`Connected!
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >/challenge/the >/challenge/planet
ssh-entrypoint: /challenge/the: Permission denied
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
29705189350862369
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{csjNO8gPv7-pSzUfxdiBf3iJwEo.dBDO0UDLyIDO0czW}`

## Reference
Copilot
