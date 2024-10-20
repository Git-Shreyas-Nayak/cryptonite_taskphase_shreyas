# finding files

## Procedure
i went to pwn.college and started the challenge.
then i went and typed `ln -s /flag /home/hacker/not-the-flag` to link between them.
Then i run the `` 
then i tried `cat` one by one.

## Code
`hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ file /flag
/flag: regular file, no read permission
hacker@commands~linking-files:~$ /home/hacker/not-the-flag
ssh-entrypoint: /home/hacker/not-the-flag: Permission denied
hacker@commands~linking-files:~$ file /home/hacker/not-the-flag
/home/hacker/not-the-flag: symbolic link to /flag
hacker@commands~linking-files:~$ cat /challenge/catflag
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{E_T-MbWKVOPbt6pIzDOP4tGUZ0h.dlTM1UDL5EjN0czW}`

## references
Nothing
