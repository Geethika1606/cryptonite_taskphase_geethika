# Helpful Programs
Connected to server, here we used --help as man page isnt available, hence --help acts as a special argument to invoke the manual. After getting the manual, following the instructions used /challenge/challenge -p 
to get the correct value to be given in -g to get the desired flag. Then gave /challenge/challenge -g 387 to get the desired flag.
***
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 387
hacker@man~helpful-programs:~$ /challenge/challenge -g 387
Correct usage! Your flag: pwn.college{oK3gtgr-IjjzuhE8NbwZeHT7vco.ddjM4QDLykjN0czW}
***
Resources used:Dojo
