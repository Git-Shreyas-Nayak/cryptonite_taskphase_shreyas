# Reading Manuals

## Procedure
i first started the challenge from pwn.collage.
then i typed `man` from mannual.
then u get a message that `--brcedv NUM print the flag if NUM is 345` .
then after typed `/challenge/challenge --brcedv 345` 

## Code
`hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                Challenge Commands                CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --brcedv NUM
              print the flag if NUM is 345

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-
       luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                      May 2024                     CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --brcedv 345
Correct usage! Your flag: pwn.college{QCbKrKcJEeXdHFHvccpqDuhza3F.dRTM4QDL5EjN0czW}`

## Reference
nothing
