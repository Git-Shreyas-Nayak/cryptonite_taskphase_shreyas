# Changing permisions

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `chmod o+r *`.
this gave the permission to read the file.
then i used cat.
then i pasted my flag to the website.

## Bash
`hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 58 Oct 12 20:20 /flag
hacker@permissions~changing-permissions:~$ chmod o+r *
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{U0dU7bu2OeujYXZmdi8MGndgdzp.dNzNyUDL5EjN0czW}`

## References
Nothing
