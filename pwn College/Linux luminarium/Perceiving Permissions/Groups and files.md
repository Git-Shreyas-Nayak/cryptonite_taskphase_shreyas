# Groups and files

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `chgrp hacker /flag`. then i saw whats inside flag by cat.
then i pasted my flag to the website.

## Bash
`hacker@permissions~groups-and-files:~$ id
uid=1000(hacker) gid=1000(hacker) groups=1000(hacker)
hacker@permissions~groups-and-files:~$ ls -l /flag
-r--r----- 1 root root 58 Oct 12 20:12 /flag
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ ls -l /flag
-r--r----- 1 root hacker 58 Oct 12 20:12 /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{0KbAO9k6PVbO20Rp_5P-LTEeEOz.dFzNyUDL5EjN0czW}`

## References
Nothing
