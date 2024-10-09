# Searching for Manuals
Connected to sever, used man man to access the man manual.Then used man -k challenge to find all the commands that reference to man.Then I opened the manual of the output and followed the instructions given in the manual to invoke the flag.
```bash
hacker@man~searching-for-manuals:~$ man man
MAN(1)                                                             Manual pager utils                                                             MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man is the system's manual pager.  Each page argument given to man is normally the name of a program, utility or function.  The manual page asso‐
       ciated with each of these arguments is then found and displayed.  A section, if provided, will direct man to look only in  that  section  of  the
       manual.   The  default  action  is  to search in all of the available sections following a pre-defined order (see DEFAULTS), and to show only the
       first page found, even if page exists in several sections.

       The table below shows the section numbers of the manual followed by the types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous (including macro packages and conventions), e.g. man(7), groff(7)
       8   System administration commands (usually only for root)
       9   Kernel routines [Non standard]

       A manual page consists of several sections.

       Conventional section names include NAME, SYNOPSIS, CONFIGURATION, DESCRIPTION, OPTIONS, EXIT STATUS, RETURN VALUE,  ERRORS,  ENVIRONMENT,  FILES,
       VERSIONS, CONFORMING TO, NOTES, BUGS, EXAMPLE, AUTHORS, and SEE ALSO.

       The following conventions apply to the SYNOPSIS section and can be used as a guide in other sections.

       bold text          type exactly as shown.
       italic text        replace with appropriate argument.
hacker@man~searching-for-manuals:~$ man -k challenge
wdvzegmwlj (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man wdvzegmwlj

CHALLENGE(1)                                                       Challenge Commands                                                       CHALLENGE(1)

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

       --wdvzeg NUM
              print the flag if NUM is 840

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                             May 2024                                                            CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --wdvzeg 840
Correct usage! Your flag: pwn.college{w8dGvzeDgOMUBmWwDlQSjKtOFBd.dZTM4QDLykjN0czW}
```
Resources used:Dojo,Had to take a little help from mentor.


