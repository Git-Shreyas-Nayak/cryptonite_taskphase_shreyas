# Executable Shell Scripts

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `touch script.sh`
then i appended `echo /challenge/solve >> script.sh`
after that i gave the permission to that and ran the script.
then i pasted my flag to the website.

## Code
`hacker@chaining~executable-shell-scripts:~$ touch script.sh
hacker@chaining~executable-shell-scripts:~$ echo /challenge/solve >> script.sh
hacker@chaining~executable-shell-scripts:~$ chmod a=rwx ./script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{UYzEYP_wJYUJGXKyOZVg5Gt_JtV.dRzNyUDL5EjN0czW}`

## References
Nothing
