# Split-piping stderr and stdout
Connected to server, used /challenge/hack > >(/challenge/planet) 2> >(/challenge/the) to get the flag. Here, I redirected from /challenge/hack to redirected to /challenge/planet and /challenge/the but instead of assigning them both the output, I assigned one of them the output using > and another the error using 2>. 
***
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{wSQQre3kZfSJ9rpxGRTjM3UJPsU.dFDNwYDLykjN0czW}
***
Resources used: Dojo
