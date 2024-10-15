# Setting path

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `PATH = "/challenge/more_commands"`
then run win .
after that u just run `/challenge/run`
then i pasted my flag to the website.

## Code
`hacker@path~setting-path:~$ pwd
/home/hacker
hacker@path~setting-path:~$ cd /challenge/more_commands
hacker@path~setting-path:/challenge/more_commands$ ls
win
hacker@path~setting-path:/challenge/more_commands$ ./win
It looks like 'win' was improperly launched. Don't launch it directly; it MUST
be launched by /challenge/run!
hacker@path~setting-path:/challenge/more_commands$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~setting-path:/challenge/more_commands$ PATH = "/challenge/more_commands"
ssh-entrypoint: PATH: command not found
hacker@path~setting-path:/challenge/more_commands$ PATH="/challenge/more_commands"
hacker@path~setting-path:/challenge/more_commands$ echo $PATH
/challenge/more_commands
hacker@path~setting-path:/challenge/more_commands$ cat flag
ssh-entrypoint: cat: command not found
hacker@path~setting-path:/challenge/more_commands$ win
It looks like 'win' was improperly launched. Don't launch it directly; it MUST
be launched by /challenge/run!
hacker@path~setting-path:/challenge/more_commands$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{gNOtEMMwbOn48TVoD4QJYM2achP.dVzNyUDL5EjN0czW}`

## References
Errors
