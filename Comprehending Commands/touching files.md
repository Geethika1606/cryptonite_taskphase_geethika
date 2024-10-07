# Touching files
Connected to the server, changed to tmp directory from home directory as the files had to be created in tmp directory. Then, I used touch to create a new file pwn and later college. Then ran /challenge/run to get the flag.
***
Connected!
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.MiOQGWw5Zc
hacker@commands~touching-files:/tmp$ touch /tmp/pwn
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.MiOQGWw5Zc
hacker@commands~touching-files:/tmp$ touch /tmp/college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.MiOQGWw5Zc
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{0SV-RsBeq0cj5bYQBfqnr8JKsaU.dBzM4QDLykjN0czW}
***
Resources used:Dojo
