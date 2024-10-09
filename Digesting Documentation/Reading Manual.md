# Reading Manuals
Connected to the server, then gave man command with challenge to access the manual connected to challenge. In the manual, figured out that --wbxenp 887 would give the flag according the instructions given. Therefore 
gave /challenge/challenge  --wbxenp 887 to invoke the flag.
```bash
Connected!
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --wbxenp NUM
              print the flag if NUM is 887

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)
hacker@man~reading-manuals:~$ /challenge/challenge  --wbxenp 887
Correct usage! Your flag: pwn.college{wbx8eUJ8Z7Tnp3si3gPASJML8C5.dRTM4QDLykjN0czW}
```
Resources used:Dojo
