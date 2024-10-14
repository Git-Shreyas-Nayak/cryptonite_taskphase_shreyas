# The SUID Bit

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `ls -l /challenge/getroot` and then i saw the permission.
after that i used `chmod u+s /challenge/getroot` to give permission for sudo.
then i pasted my flag to the website.

## Code
`hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwxr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# ls -l /challenge/getroot
-rwsr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
root@permissions~the-suid-bit:~# cat /flag
pwn.college{0rXypVweFKe-14HoHBpfsCAodRb.dNTM2QDL5EjN0czW}`

## References
Nothing
