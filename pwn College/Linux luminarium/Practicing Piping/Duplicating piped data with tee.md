# Duplicating piped data with tee

## Procedure
i started the challenge `pwn.college`
then i typed `/challenge/pwn | tee temp | /challenge/college` , this stores the value of /challenge/pwn to tmp .
then `cat tmp` , this tells about the contents in it.
so we needto put the secret key to access the /challenge/college.
hence i wrote `/challenge/pwn --secret EDmy38z3 | /challenge/college`
as this does both the commands live.
the i pasted my flag to the website.

## Code
`hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee temp | /challeng
e/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat temp
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "EDmy38z3"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret EDmy38z3 | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{EDmy38z3fJPJDZDIw9l7wyF8P6R.dFjM5QDL5EjN0czW}`

## References
Errors
