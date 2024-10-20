# bandit 5 --> 6

## Procedure
i started the challenge by reading in OverTheWire.
then i went to the terminal and connected to it.
by putting ssh bandit @bandit5.labs.overthewire.org -p 2220 
and password as `4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw`
then i typed `find . -type f -size 1033c -exec file {} \; | grep -i 'text' | grep -v 'executable'`.
this finds the file which has size 1033c which is not executable and is in text.
then i catted out the file which i got `cat ./maybehere07/.file2`.
then i noted the password `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`.
after that i typed exit to get of the shell.

## bash
`bandit5@bandit:~$ cd inhere
bandit5@bandit:~/inhere$ find . -type f -size 1033c -exec file {} \; | grep -i 'text' | grep -v 'executable'
./maybehere07/.file2: ASCII text, with very long lines (1000)
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

## Reference
Copilot
