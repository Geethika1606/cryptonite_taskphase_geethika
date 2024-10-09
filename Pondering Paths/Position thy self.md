# Position thy self
Linked to the server and then typed /challenge/run to find out which directory the linux is supposed to be a part of. /usr/bin was the desired directory hence changed to it using the cd command and then invoked
/challenge/run to get the desired flag.
```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/bin directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/bin
hacker@paths~position-thy-self:/usr/bin$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Q_CvTo8P8vljgqlCj_cDMHmstG2.dZDN1QDLykjN0czW}
hacker@paths~position-thy-self:/usr/bin$
```
Resources used:Dojo
