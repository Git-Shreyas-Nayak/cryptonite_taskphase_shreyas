# Position thy self

## Procedure
I went to pwn.college and started the challenge of The root.
Then i went to ubuntu and typed `/challenge/run`.
then i got a incorrect message saying `cd` to change directory to `/home`
hence i typed `cd /home` to get inside directory.
then i typed `/challenge/run`.
After that i got the flag and pasted in the pwn.college.

## Code
`hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /home directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /home
hacker@paths~position-thy-self:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{kkU799Int1DR2hJIxoodJR6ppMQ.dZDN1QDL5EjN0czW}`

## Reference
The invalid answer from the prompt
