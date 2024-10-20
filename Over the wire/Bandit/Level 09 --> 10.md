# Level 9 --> 10

## Procedure
i started the challenge by reading in OverTheWire.
then i went to the terminal and connected to it.
by putting `ssh bandit @bandit9.labs.overthewire.org -p 2220` 
and password as `4CKMh1JI91bUIZZPXDqGanal4xvAg0JM`
then i typed `strings data.txt | grep '======'`.
then i noted the password `FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`.
after that i typed exit to get of the shell.

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
