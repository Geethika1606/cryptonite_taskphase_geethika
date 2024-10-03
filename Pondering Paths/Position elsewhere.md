# Position elsewhere
Linked to the server, ran /challenge/run to figure out which directory to redirect to. Redirected to /proc/67 using cd command and invoked /challenge/run from it.
***
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/67 directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /proc/67
hacker@paths~position-elsewhere:/proc/67$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{8SdzH9rQlJ60FNOyyQlDJoGRQyr.ddDN1QDLykjN0czW}
***
Resources used:Dojo
