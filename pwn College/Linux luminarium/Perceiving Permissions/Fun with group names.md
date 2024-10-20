# Fun with group names

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `id`.
this gave me the name `grp2286`.
then i used ` chgrp grp2286 /flag`.
after that cat.
then i pasted my flag to the website.

## Bash
`hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp2286) groups=1000(grp2286)
hacker@permissions~fun-with-groups-names:~$ ls -l /flag
-r--r----- 1 root root 58 Oct 12 20:16 /flag
hacker@permissions~fun-with-groups-names:~$ chgrp grp2286 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{wUDywOVHzltdULTiLlkGcdK-utI.dJzNyUDL5EjN0czW}`

## References
Nothing
