# Explicit relative paths,from /
Connected to the server and used cd/challenge and./run to determine the desired directory. In the desired directory, gave ./challenge/run to get a relative path and got the flag.
***
Connected!
hacker@paths~explicit-relative-paths-from-:~$ cd /challenge
hacker@paths~explicit-relative-paths-from-:/challenge$ ./run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:/challenge$ /
ssh-entrypoint: /: Is a directory
hacker@paths~explicit-relative-paths-from-:/challenge$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{EY8wJ6KlnfZLHf2TDQeZW6e3zRH.dBTN1QDLykjN0czW}
***
Resources used: Dojo
