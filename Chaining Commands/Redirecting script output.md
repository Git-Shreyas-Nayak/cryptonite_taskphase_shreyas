# Redirecting script output

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `touch hey2.sh`.
then as the last challenges i appended both.
after that i piped like this `bash hey2.sh | /challenge/solve`
then i pasted my flag to the website.

## Code
`hacker@chaining~redirecting-script-output:~$ touch hey2.sh
hacker@chaining~redirecting-script-output:~$ echo /challenge/pwn >> hey2.sh
hacker@chaining~redirecting-script-output:~$ echo /challenge/college >> hey2.sh
hacker@chaining~redirecting-script-output:~$ bash hey2.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{8YnM6KlfN3nmFjxkOSMLb3Jz3gC.dhTM5QDL5EjN0czW}`

## References
Nothing
