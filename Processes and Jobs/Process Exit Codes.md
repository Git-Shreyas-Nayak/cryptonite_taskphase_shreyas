# Process Exit Codes

## Procedure
i started the challenge pwn.college
as per the question.
then i typed `/challenge/get-code`.
to see the code i typed `echo $?`
then after getting to know the code and the format how to write ,
i typed `/challenge/submit-code 231`
then i pasted my flag to the website.

## Code
`hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
231
hacker@processes~process-exit-codes:~$ 231 > /challenge/submit-code
ssh-entrypoint: /challenge/submit-code: Permission denied
hacker@processes~process-exit-codes:~$ /challenge/submit-code
You must run /challenge/submit-code with the exit code you retrieved from
/challenge/get-code as the first argument:

Usage: /challenge/submit-code [EXIT_CODE]
hacker@processes~process-exit-codes:~$ /challenge/submit-code 231
CORRECT! Here is your flag:
pwn.college{E_EKfQXfcQRFEnLsZ60pwPSF7jD.dljN4UDL5EjN0czW}`

## References
Errors
