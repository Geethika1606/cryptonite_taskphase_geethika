# Help for Builtins
Connected to server, used help challenge to open challenge manual and used --secret 0n4n_4QG to invoke flag as per the instructions.
***
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "0n4n_4QG".
hacker@man~help-for-builtins:~$ challenge  --secret 0n4n_4QG
Correct! Here is your flag!
pwn.college{0n4n_4QG-_rI3iYqd8Ivjcy-nzf.dRTM5QDLykjN0czW}
***
Resources used:Dojo
