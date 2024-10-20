# Matching with []

## Procedure
i started the challenge 'pwn.college'
then i typed `cd /challenge/files`.
as it told  only 4 char can be put so typed `ls`.
then ran the flag `/challenge/files$ /challenge/run file_[hasb]`.
the i pasted my flag to the website.

## Code
`hacker@globbing~matching-with-:~$ cd /challe[nge]
ssh-entrypoint: cd: /challe[nge]: No such file or directory
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ ls
file_a  file_d  file_g  file_j  file_m  file_p  file_s  file_v  file_y
file_b  file_e  file_h  file_k  file_n  file_q  file_t  file_w  file_z
file_c  file_f  file_i  file_l  file_o  file_r  file_u  file_x
hacker@globbing~matching-with-:/challenge/files$ files_[]./run
ssh-entrypoint: files_[]./run: No such file or directory
hacker@globbing~matching-with-:/challenge/files$ /challenge/run
Error: you did not use a square bracket glob...
hacker@globbing~matching-with-:/challenge/files$ /challenge/run ./file_[bash]
Your expansion did not expand to the requested files (file_a, file_b, file_h,
and file_s). Instead, it expanded to:
./file_a ./file_b ./file_h ./file_s
hacker@globbing~matching-with-:/challenge/files$ /challenge/run /challenge/f
ile_[bash]
Your expansion did not expand to the requested files (file_a, file_b, file_h,
and file_s). Instead, it expanded to:
/challenge/file_[bash]
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[hasb]
You got it! Here is your flag!
pwn.college{0tCvPJVjFMjSTgHgNTXaBgW9L00.dNjM4QDL5EjN0czW}`

## References
Errors
