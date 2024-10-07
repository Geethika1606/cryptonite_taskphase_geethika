# Listing files
Connected to the server, used ls command with challenge argument to figure out what /challenge/run is renamed as. Used the renamed path to invoke the flag.
***
hacker@commands~listing-files:~$ ls /challenge
28578-renamed-run-13884  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/28578-renamed-run-13884
Yahaha, you found me! Here is your flag:
pwn.college{UhNZfpU9FUo3VrNpEPs2t7xs4rp.dhjM4QDLykjN0czW}}
***
Resources used: Dojo
