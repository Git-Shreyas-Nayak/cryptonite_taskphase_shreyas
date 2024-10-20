# Backgrounding processes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `/challenge/run` and then terminate it as per told.
then i opened a new terminal and typed `/challenge/run`
then i went to the first one and started running again so i stopped agin using `ctrl+z`.
then i typed `bg /challenge/run`
then i pasted my flag to the website.

## Code
`hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root          82 S+   bash /challenge/run
root          84 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg /challenge/run
[1]+ /challenge/run &



Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root          82 S    bash /challenge/run
root         109 S    sleep 6h
root         110 S+   bash /challenge/run
root         112 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{0QUskc6dsFlLLTmvxuC23AiidcY.ddDN4QDL5EjN0czW}`

## References
Nothing
