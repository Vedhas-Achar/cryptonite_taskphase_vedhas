# Suspending Process

## Procedure
I started the challenges and then connected to my terminal<br>
then i used ran `/challenge/run` and then used `Ctrl-Z` to suspend it and then ran
`/challenge/run` and then got the flag which i then pasted into the flag box.

## bash
`Connected!
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!
UID          PID    PPID  C STIME TTY          TIME CMD
root          83      66  0 13:22 pts/0    00:00:00 bash /challenge/run
root          85      83  0 13:22 pts/0    00:00:00 ps -f
I don't see a second me!
To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!
UID          PID    PPID  C STIME TTY          TIME CMD
root          83      66  0 13:22 pts/0    00:00:00 bash /challenge/run
root          90      66  0 13:22 pts/0    00:00:00 bash /challenge/run
root          92      90  0 13:22 pts/0    00:00:00 ps -f
Yay, I found another version of me! Here is the flag:
pwn.college{YfGw_vDwTpmHOJsNdFn8XGDe1H6.dVDN4QDLyIDO0czW}`

## Reference
Didnt use
