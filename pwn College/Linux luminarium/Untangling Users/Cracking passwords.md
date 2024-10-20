
# Cracking passwords

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `john /challenge/shadow-leak`
then i pasted my flag to the website.

## Bash
`hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:13 0% 2/3 0g/s 283.7p/s 283.7c/s 283.7C/s bigdog..francesco
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04894g/s 285.0p/s 285.0c/s 285.0C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
aardvarkhacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{0PD21JpJxsVlJq7vR3ZZ0Ai2hw-.ddTN0UDL5EjN0czW}`

## References
Nothing
