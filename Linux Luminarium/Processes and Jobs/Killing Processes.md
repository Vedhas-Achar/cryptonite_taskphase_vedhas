# Killing Processes

## Procedure
i started the challenge and then connected the terminal<br>
after that i used `ps -e | grep sleep` and got the PID number, which i killed using `kill 74` and then got the flag, which i pasted into flag box.

## bash
`Connected!
hacker@processes~killing-processes:~$ ps -e | grep /challenge/dont_run
hacker@processes~killing-processes:~$ ps -e | grep sleep
     74 ?        00:00:00 sleep
hacker@processes~killing-processes:~$ kill 74
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{MPUz6o9M1XZ67XjOmrq0IgPWBl9.dJDN4QDLyIDO0czW}`

## Reference
Didnt use
