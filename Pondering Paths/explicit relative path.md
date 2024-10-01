# explicit relative paths

## procedure
first i started the code challenge in pwn.college.
then as per the question i wrote `./challenge/run`.
but as no directory is given i went back with `cd ..` 2 times.
then typed `./challenge/run` again.
after that i pasted the flag in the pwn.collage.

## code
`hacker@paths~explicit-relative-paths-from-:~$ ./challenge/run
ssh-entrypoint: ./challenge/run: No such file or directory
hacker@paths~explicit-relative-paths-from-:~$ pwd
/home/hacker
hacker@paths~explicit-relative-paths-from-:~$ cd ..
hacker@paths~explicit-relative-paths-from-:/home$ cd ..
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{w1_tbNRyZZ3_DpTwmJSMLYOiM8u.dBTN1QDL5EjN0czW}`

# reference
real friends
