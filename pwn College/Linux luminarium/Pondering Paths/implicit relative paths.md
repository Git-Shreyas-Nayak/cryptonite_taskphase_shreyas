# implicit relative paths

## procedure
first i started the code challenge in pwn.college.
then as per the question i did not add the start / and wrote `challenge/run`.
but as no directory is given i went back with `cd ..` 2 times and typed ls .
then typed `cd challenge`. after that i typed `./run`.
after that i pasted the flag in the pwn.collage.

## code
`hacker@paths~implicit-relative-path:~$ cd ..
hacker@paths~implicit-relative-path:/home$ cd ..
hacker@paths~implicit-relative-path:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@paths~implicit-relative-path:/$ cd challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{QYU_9rbG0WlaQwC5mD2XbCxMnER.dFTN1QDL5EjN0czW}`

# reference
my errors,friends
