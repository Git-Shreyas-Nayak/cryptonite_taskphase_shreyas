# Redirecting input

## Procedure
i started the challenge `pwn.college`
then i typed `echo COLLEGE > PWN` as per the question.
then after that `/challenge/run < PWN`.
the i pasted my flag to the website.

## Code
`hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ cat PWN
COLLEGE
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{wPzAGsDz7XO3enYrPXzJ7aiFm7_.dBzN1QDL5EjN0czW}`

## References
Nothing
