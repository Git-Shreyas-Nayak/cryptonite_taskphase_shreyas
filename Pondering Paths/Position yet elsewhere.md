# Position yet elsewhere

## Procedure
I went to pwn.college and started the challenge of The root.
Then i went to ubuntu and typed `/challenge/run`.
then i got a incorrect message saying `cd` to change directory to `/usr/bin`
hence i typed `cd /usr/bin` to get inside directory.
then i typed `/challenge/run`.
After that i got the flag and pasted in the pwn.college.

## Code
`hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/bin directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/bin
hacker@paths~position-yet-elsewhere:/usr/bin$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{IEliZgfiwfipw2Xo8w89_JS85ME.dhDN1QDL5EjN0czW}`

## Reference
nothing
