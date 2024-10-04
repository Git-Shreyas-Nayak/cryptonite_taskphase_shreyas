# making directories

## Procedure
first i started the challenge from `pwn.college` and went to the terminal.
then i got to know about `mkdir` and `touch`.
then i run the `/challenge/run`.

## Code
`hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ cd /pwn
ssh-entrypoint: cd: /pwn: No such file or directory
hacker@commands~making-directories:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.G9qthVCks5
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ cd ..
hacker@commands~making-directories:/tmp$ cd pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{gAigvgBY3heN1qhJfIIkorFkTNg.dFzM4QDL5EjN0czW}`

## Reference
nothing
