# Searching Manual

## Procedure
i started by starting the challenge in `pwn.college`.
then i typed `man man`.
then reaaaaaaad everything .
then u get to know about `-k`
then i executed `man -K pwn.college`.
then type `/challenge/challenge --kvinpt 281`
then i pasted my flag in the website.

## Code
`hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -K pwn.college

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

       --kvinpt NUM
              print the flag if NUM is 281

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-
       luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                      May 2024                     CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --kvinpt 281
Correct usage! Your flag: pwn.college{kviLnptOIQ2T8xDIeYZRt1RWmU-.dZTM4QDL5EjN0czW}`

## Reference
Errorsss
