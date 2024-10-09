# Grepping stored result

## Procedure
i started the challenge `pwn.college`
then i typed `/challenge/run > /tmp/data.txt`
after the output is being redirected.
then as per the info i needed to grep.
hence i did `grep pwn /tmp/data.txt`
the i pasted my flag to the website.

## Code
`hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep flag /tmp/data.txt
[FLAG] Here is your flag:
flagon
flagellating
flagrantly
flagellated
flagellation's
camouflaged
persiflage's
flagellates
flagpole's
flagellate
conflagrations
flagrant
conflagration
conflagration's
camouflage's
flagon's
flagellums
flagstaff
flagstone
flagella
camouflage
flagship's
flagstaffs
flagship
flag
flagged
flagstones
flagstaff's
flagellation
flag's
flagging
flagpoles
camouflages
flagpole
camouflaging
persiflage
flagellum's
unflagging
flagellum
flagships
flagons
flagstone's
flags
hacker@piping~grepping-stored-results:~$ grep pwn /tmp/data.txt
pwning
pwn
pwned
pwns
pwn.college{sKtRWQon2xmKDRRPa12T8bWoMrM.dhTM4QDL5EjN0czW}`

## References
Nothing
