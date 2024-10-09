# Writing to multiple programs
Connected to server, used /challenge/hack | tee >(/challenge/the) | tee >(/challenge/planet) to get the flag. Here /challenge/hack's output is being redirected to the input of /challenge/the and the /challenge/planet commands
using >() and tee. Tee is used to intercept the data while >() is used to substitute the data.
```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) | tee >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
29668135861691621519
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{cCHtzCZ3fpcGq97bb8q_gDWpV9X.dBDO0UDLykjN0czW}
```
Resiurces used:Dojo
