# bandit 6-7

## Procedure
I connected my terminal, then i used `cd /` , then i used `find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null`
to find file which was owned by group 7 or 6, and had size of 33c and permissions which were not denied, and got the file i was looking for, i then catted it which gave me the flag.

## bash
`bandit6@bandit:/$ find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:/$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`

## Reference
Copilot
