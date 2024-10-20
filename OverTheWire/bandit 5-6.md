# bandit 5-6

## Procedure
I connected my terminal<br>
then i used `cd inhere` and then used `find . -type f -size 1033c -exec file {} \; | grep -i 'text' | grep -v 'executable'`
and then used `cat ./maybehere07/.file2` and then got the password.

## bash
`bandit5@bandit:~$ cd inhere
bandit5@bandit:~/inhere$ find . -type f -size 1033c -exec file {} \; | grep -i 'text' | grep -v 'executable'
./maybehere07/.file2: ASCII text, with very long lines (1000)
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

## Reference
Didnt use
