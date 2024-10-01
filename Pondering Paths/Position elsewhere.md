# Position elsewhere

## Procedure
I went to pwn.college and started the challenge of The root.
Then i went to ubuntu and typed `/challenge/run`.
then i got a incorrect message saying `cd` to change directory to `/tmp`
hence i typed `cd /tmp` to get inside directory.
then i typed `/challenge/run`.
After that i got the flag and pasted in the pwn.college.

## Code
`hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /tmp
hacker@paths~position-elsewhere:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Esepgd3YxbYyJy7k-W6IfLOOcjE.ddDN1QDL5EjN0czW}`

## Reference
nothing
