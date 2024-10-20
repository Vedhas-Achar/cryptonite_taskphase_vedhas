# bandit 9-10

## Procedure
I connected my terminal, then i used my logic, and then it failed, then used copilot logic
`strings data.txt | grep '===='`
and then got the flag

## bash
`bandit9@bandit:~$ grep "==" data.txt
grep: data.txt: binary file matches
bandit9@bandit:~$ strings data.txt | grep '======'
}========== the
3JprD========== passwordi
~fDV3========== is
D9========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`

## Reference
Copilot
