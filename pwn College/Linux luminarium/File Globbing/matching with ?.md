# matching with ?

## Procedure
i started the challenge 'pwn.college'
then i typed `cd /challeng?`.
as it told u cant use `*,c,l` char can be put so typed `cd /?ha??enge`.
then ran the flag `./flag`.
the i pasted my flag to the website.

## Code
`hacker@globbing~matching-with-:~$ cd /challeng?
You used either the 'c', 'l', or '*' characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ ./run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{EtD6peerReLlkUmQUcRI26sS601.dJjM4QDL5EjN0czW}`

## References
this thing is there in python as `_`
