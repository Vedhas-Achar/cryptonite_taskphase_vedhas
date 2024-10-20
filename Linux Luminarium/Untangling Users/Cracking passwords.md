# Cracking passwords

## Procedure
I started the challenge, and then connected my terminal<br>
then i used `john /challenge/shadow-leak` and got the password of zardus user,
then i used `su zardus` to get the shell, then ran `/challenge/run` to get my flag.
(ps. this was the most hacker vibe i felt)

## bash
`Connected!
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04868g/s 283.4p/s 283.4c/s 283.4C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{c7JYVtZ2wn9JD5nge-CiA9oVg3R.ddTN0UDLyIDO0czW}`

## Reference
Didnt use
