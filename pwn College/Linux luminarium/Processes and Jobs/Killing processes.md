# Killing processes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `ps -ef | grep dont_run`
after grtting the number now we hould kill it.
hence type `kill 73`.
now run the `/challenge/run`
then i pasted my flag to the website.

## Code
`hacker@processes~killing-processes:~$ ps -ef | grep dont_run
hacker        73      71  0 18:24 ?        00:00:00 /challenge/dont_run
hacker       116      81  0 18:27 pts/0    00:00:00 grep --color=auto dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{YMWypQUUjaoeJv4Tf5GqUyAO0Xa.dJDN4QDL5EjN0czW}`

## References
Errors
