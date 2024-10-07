# Hidden files
Connected to the server, used ls -a as directed to get files that are hidden as they start with a '.' . The hidden files gave a flag arguement which i used with cat command to invoke the flag.
***
hacker@commands~hidden-files:~$ ls -a /
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-31370714416692  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:~$ cat /.flag-31370714416692
pwn.college{4d8NTf74nffGa_X0kWgpchUnJO5.dBTN4QDLykjN0czW}
***
Resources used:Dojo
