# Suspending processes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `/challenge/run`
then as it asked me to open an another teminal i did and `ctrl+z` in the first to stop
also in the second i ran `/challenge/run` and in the previous one i ran `/challenge/run again`
then i pasted my flag to the website.

## Code
`hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in

this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 18:33 pts/0    00:00:00 bash /challenge/run
root         113      65  0 18:34 pts/0    00:00:00 bash /challenge/run
root         115     113  0 18:34 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{oTqhPSv-prdIAxEnnGAu6fgJ6pm.dVDN4QDL5EjN0czW}`

## References
Nothing
