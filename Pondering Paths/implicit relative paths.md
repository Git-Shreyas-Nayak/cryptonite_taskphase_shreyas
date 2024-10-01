# implicit relative paths

## procedure
first i started the code challenge in pwn.college.
then as per the question i did not add the start / and wrote `challenge/run`.
but as no directory is given i went back with `cd ..`
then typed `challenge/run` again.
after that i pasted the flag in the pwn.collage.

## code
`hacker@paths~implicit-relative-paths-from-:~$ challenge/run
ssh-entrypoint: challenge/run: No such file or directory
hacker@paths~implicit-relative-paths-from-:~$ cd ..
hacker@paths~implicit-relative-paths-from-:/home$ challenge/run
ssh-entrypoint: challenge/run: No such file or directory
hacker@paths~implicit-relative-paths-from-:/home$ cd ..
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{IUDcyNZFnshjDup92LOQHwLtKsF.dlDN1QDL5EjN0czW}`

# reference
my errors
