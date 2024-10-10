# Listing processes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `ps -ef`
there was a challenge statemnent runned so even i typed it.
then i pasted my flag to the website.

## Code
`hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 18:16 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 18:16 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 18:16 ?        00:00:00 /challenge/5910-run-13514
root          72      68  0 18:16 ?        00:00:00 sleep 6h
hacker        73       0  0 18:16 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90       0  0 18:16 pts/1    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker       112      90  0 18:20 pts/1    00:00:00 ps -ef
hacker@processes~listing-processes:~$ [200~/challenge/5910-run-1351~
ssh-entrypoint: [200~/challenge/5910-run-1351~: No such file or directory
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 18:16 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 18:16 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 18:16 ?        00:00:00 /challenge/5910-run-13514
root          72      68  0 18:16 ?        00:00:00 sleep 6h
hacker        73       0  0 18:16 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90       0  0 18:16 pts/1    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker       114      90  0 18:20 pts/1    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/5910-run-13514
Yahaha, you found me! Here is your flag:
pwn.college{wARZJdZSAKo2lNdcvTYA0_KTofG.dhzM4QDL5EjN0czW}
Now I will sleep for a while (so that you could find me with 'ps').`

## References
Nothing
