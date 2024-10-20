# bandit 6 --> 7

## Procedure
i started the challenge by reading in OverTheWire.
then i went to the terminal and connected to it.
by putting ssh bandit `@bandit6.labs.overthewire.org -p 2220` 
and password as `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`
then i typed `find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null`.
then i catted out with the address as `cat /var/lib/dpkg/info/bandit7.password`
then i noted the password `morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`.
after that i typed exit to get of the shell.

## bash
`bandit6@bandit:/$ find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:/$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`

## Reference
Copilot
