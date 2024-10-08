# Redirecting errors
Connected to the server, used /challenge/run > myflag 2> instructions to redirect. First in this statement, /challenge/run > myflag redirects to output. The latter part, 2> instructions is used to redirect errors.
Then used ls command with myflag to find list in it. Used cat command with myflag to invoke the flag.
***
Connected!
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ ls myflag
myflag
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{c-Kh_5k0l_LJmKnjNeGXRGFL1h1.ddjN1QDLykjN0czW}
***
Resources used:Dojo
