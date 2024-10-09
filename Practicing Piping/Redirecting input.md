# Redirecting input
Connected to the server, used echo to give an output from COLLEGE to PWN. Then I redirected to PWN using < and /challenge/run to invoke the required flag.
***
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{4946-fLPwSmf5kcZd7DqhS1Hn5l.dBzN1QDLykjN0czW}
***
Resources used:Dojo
