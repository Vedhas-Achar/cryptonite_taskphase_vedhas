# Listing Processes

## Procedure
I started the challenge and then connected my terminal<br>
Then i used `ps aux` and got the processes, but i tried all of them and
didnt get the answer, then i got to know that my paths were truncated,
hence i extended the screen , and this time i got `/challenge/5185-run-24710` and
got the flag.

## bash
`hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.5  0.0   1056   640 ?        Ss   12:20   0:00 /sbin/doc
root           7  0.0  0.0   5052  2560 ?        S    12:20   0:00 /run/dojo
root          68  0.0  0.0   4132  2560 ?        S    12:20   0:00 /challeng
root          72  0.0  0.0   2744  1600 ?        S    12:20   0:00 sleep 6h
hacker        73  0.8  0.0   5360  3840 pts/0    Ss   12:20   0:00 /run/dojo
hacker        90  0.0  0.0   7868  3520 pts/0    R+   12:20   0:00 ps aux
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.3  0.0   1056   640 ?        Ss   12:20   0:00 /sbin/docker-init -- /nix/var/nix/
root           7  0.0  0.0   5052  2560 ?        S    12:20   0:00 /run/dojo/bin/sleep 6h
root          68  0.0  0.0   4132  2560 ?        S    12:20   0:00 /challenge/5185-run-24710
root          72  0.0  0.0   2744  1600 ?        S    12:20   0:00 sleep 6h
hacker        73  0.2  0.0   5360  3840 pts/0    Ss   12:20   0:00 /run/dojo/bin/ssh-entrypoint
hacker        91  0.0  0.0   7868  3200 pts/0    R+   12:21   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/5185-run-24710
Yahaha, you found me! Here is your flag:
pwn.college{gg39xG_eKhI7UtdIF2oT1zoLkda.dhzM4QDLyIDO0czW}
Now I will sleep for a while (so that you could find me with 'ps').`

## Reference
Friend
