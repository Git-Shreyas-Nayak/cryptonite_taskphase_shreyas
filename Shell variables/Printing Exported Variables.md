# Printing Exported Variables

## Procedure
i started the challenge `pwn.college`
as per the question.
then i typed `env pwn`
then i got a list of pwn variable values.
so to search in them i used grep `env | grep pwn`
the i pasted my flag to the website.

## Code
`hacker@variables~printing-exported-variables:~$ env FLAG
env: ‘FLAG’: No such file or directory
hacker@variables~printing-exported-variables:~$ env pwn
usage: pwn [-h]
           {asm,checksec,constgrep,cyclic,debug,disasm,disablenx,elfdiff,elfpatch,errno,hex,libcdb,phd,pwnstrip,scramble,shellcraft,template,unhex,update,version}
           ...
hacker@variables~printing-exported-variables:~$ env | grep pwn
FLAG=pwn.college{gDgJoq-a19cLSO-mcMVQYZmHbYJ.dhTN1QDL5EjN0czW}`

## References
Errors and friends
