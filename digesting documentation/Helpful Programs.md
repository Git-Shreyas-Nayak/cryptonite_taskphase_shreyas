# Helpful Programs

## Procedure
i started by starting the challenge in `pwn.college`.
then i typed `/challenge/challenge help`.
then read everything .
then i wanted thr print so i did this `/challenge/challenge -p`.
then i executed `/challenge/challenge -g 44`.
then i pasted my flag in the website.

## Code
`hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to
                        give you the flag
hacker@man~helpful-programs:~$ challenge/challenge -p
ssh-entrypoint: challenge/challenge: No such file or directory
hacker@man~helpful-programs:~$ challenge/challenge --p
ssh-entrypoint: challenge/challenge: No such file or directory
hacker@man~helpful-programs:~$ challenge/challenge -g
ssh-entrypoint: challenge/challenge: No such file or directory
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 44
hacker@man~helpful-programs:~$ /challenge/challenge -g 44
Correct usage! Your flag: pwn.college{gSHb0OKFsgM_kpgrijZjhKSIBp4.ddjM4QDL5EjN0czW}`

## Reference
Errorsss 
