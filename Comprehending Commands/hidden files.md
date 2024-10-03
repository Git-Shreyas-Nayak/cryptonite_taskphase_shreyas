# hidden files

## Procedure
first i started the challenge from `pwn.college` and went to the terminal.
as per the website i searched `ls -a`. then i got the hidden thing.
then i typed ` cat .flag-28760110953422`.
then i pasted the flag in the site.

## Code
`hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.                     bin        etc    lib64   nix   run   tmp
..                    boot       home   libx32  opt   sbin  usr
.dockerenv            challenge  lib    media   proc  srv   var
.flag-28760110953422  dev        lib32  mnt     root  sys
hacker@commands~hidden-files:/$ cat .flag-28760110953422
pwn.college{cnKPNNbHTrfsFo1ArE0fRWTaBYj.dBTN4QDL5EjN0czW}`

## Reference
Nothing
