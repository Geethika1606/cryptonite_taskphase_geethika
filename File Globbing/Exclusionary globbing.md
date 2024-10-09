# Exclusionary globbing
Connected to the server, used cd to change from home directory to /challenge/files directory.Then used ls command to list the files in the directory and then gave  /challenge/run [!pwn]* to get
flag.
```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ ls
amazing      delightful   great       jovial    magical     pwning   splendid   victorious  youthful
beautiful    educational  happy       kind      nice        queenly  thrilling  wonderful   zesty
challenging  fantastic    incredible  laughing  optimistic  radiant  uplifting  xenial
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{YuVLvcbUyb6NqNOBLxa00yxljy-.dZjM4QDLykjN0czW}
```
Resources used:Dojo
