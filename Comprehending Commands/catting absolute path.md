# catting absolute path

## Procedure
i started the challenge, then connected terminal. 
i found that i was in `/home/hacker` hence i went to `/`. 
then i knew that my flag was in `/flag`.
hence i used `cat /flag` to get the answer.

## bash
`Connected!
hacker@commands~catting-absolute-paths:~$ cat /file
cat: /file: No such file or directory
hacker@commands~catting-absolute-paths:~$ pwd
/home/hacker
hacker@commands~catting-absolute-paths:~$ cd /
hacker@commands~catting-absolute-paths:/$ pwd
/
hacker@commands~catting-absolute-paths:/$ cat /file
cat: /file: No such file or directory
hacker@commands~catting-absolute-paths:/$ cat cat /flag
cat: cat: No such file or directory
pwn.college{cf8cDTloT4J8EYUNBbcJHVSBAd4.dlTM5QDLyIDO0czW}
hacker@commands~catting-absolute-paths:/$ pwd
/
hacker@commands~catting-absolute-paths:/$ cat /flag
pwn.college{cf8cDTloT4J8EYUNBbcJHVSBAd4.dlTM5QDLyIDO0czW}`

## Reference
Didnt use
