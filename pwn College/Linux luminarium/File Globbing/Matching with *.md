# Matching with *

## Procedure
i started the challenge 'pwn.college'
then i typed `cd /chall*`.
as it told  only 4 char can be put so typed `cd /c*`.
then ran the flag `./flag`.
the i pasted my flag to the website.

## Code
`This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /chall*
You specified the path to 'cd' to in more than 4 characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ ./run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{U-NZBhJWCTvusXOKmVQUnEDErsW.dFjM4QDL5EjN0czW}`

## References
this thing is there in python
