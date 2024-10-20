# Foregrounding processes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `/challenge/run` and stopped it by `ctrl+z`
in another teminal again i typed `/challenge/run` and we ahould not stop this
back to the previous terminal i typed `fg /challenge/run`
then it gave me the message.
after reading that i stopped it and typed `bg challenge/run`.
so at last i terminated for the last time and wrote `fg /challenge/run`
then i pasted my flag to the website.

## Code
`hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ fg /challenge/run
/challenge/run
You resumed me into the foreground from suspension! Please resume me into the
background, and *then* swap me into the foreground directly from there (or
press Enter, and I'll exit).
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg /
challenge/run
[1]+ /challenge/run &



Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
hacker@processes~foregrounding-processes:~$ fg /
challenge/run
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!
hacker@processes~foregrounding-processes:~$
pwn.college{Ade-U-_RJ2T17277ch6QiZCobgj.dhDN4QDL5EjN0czW}`

## References
Errors
