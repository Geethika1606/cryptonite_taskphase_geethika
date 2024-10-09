# Duplicating piped data with tee
Connected to the server, First I intercepted with tee to find out the secret code and then added the secret code to /challenge/pwn | tee /challenge/run_ouput | /challenge/college and intercepted again to get the 
desired flag.
***
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee /challenge/run_ouput | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat /challenge/run_ouput
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "Y-Ozy51n"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret Y-Ozy51n | tee /challenge/run_ouput | /challenge/college
Processing...
WARNING: you are overwriting file /challenge/run_ouput with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{Y-Ozy51nCkUZ4g0vty83FpyX2NG.dFjM5QDLykjN0czW}
***
Resources used:Dojo, Had to ask my mentor for help
