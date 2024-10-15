# Adding commands

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `#!/bin/bash' > win`
after that `echo 'cat /flag' >> ~/win` and this will append the cat/flag in win.
after that then i type `PATH=~/:$PATH` 
then i ran it.
then i pasted my flag to the website.

## Code
`hacker@path~adding-commands:~$ #!/bin/bash' > win
hacker@path~adding-commands:~$ echo 'cat /flag' >> ~/win
hacker@path~adding-commands:~$ chmod +x ~/win
hacker@path~adding-commands:~$ PATH=~/:$PATH
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{UVGYPvD30T4BwYrfUPTpOBfrzhl.dZzNyUDL5EjN0czW}`

## References
AI
