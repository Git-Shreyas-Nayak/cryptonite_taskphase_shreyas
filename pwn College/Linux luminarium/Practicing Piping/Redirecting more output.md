# Redirecting more output

## Procedure
i started the challenge `pwn.college`
then i typed `/challenge/run > myflag` To redirect the file in /challenge/run.
then as per the info printed after this .
i had to see what was inside the file.
hence i did `cat myflag`
the i pasted my flag to the website.

## Code
`hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ ls
COLLEGE  a  myflag  not-the-flag
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oJ3bQrULlASNYCAamc3WVxdNQAR.dVjN1QDL5EjN0czW}`

## References
Errors
