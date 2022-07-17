# Task 3 - Intro to Flags and Switches

- A majority of commands allow for arguments to be provided. 

- These arguments are identified by a hyphen and a certain keyword known as flags or switches.

- When using a command, unless otherwise specified, it will perform its default behaviour. 

- For example, `ls` lists the contents of the working directory. 

- However, hidden files are not shown. 

- We can use flags and switches to extend the behaviour of commands.

Using our `ls` example, ls informs us that there is only one folder named `"folder1"` as highlighted in the screenshot below. 

Note that the contents in the snippets below are only examples.

```        
tryhackme@linux2:~$ ls
folder1
tryhackme@linux2:~$
```

However, after using the `-a` argument (short for `--all`), we now suddenly have an output with a few more files and folders such as `".hiddenfolder"`. 

Files and folders with `"."` are hidden files.

```   
tryhackme@linux2:~$ ls -a 
.hiddenfolder folder1
tryhackme@linux2:~$
```

Commands that accept these will also have a `--help` option. 

This option will list the possible options that the command accepts, provide a brief description and example of how to use it.

```           
tryhackme@linux2:~$ ls --help
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all                  do not ignore entries starting with .
  -A, --almost-all           do not list implied . and ..
      --author               with -l, print the author of each file
  -b, --escape               print C-style escapes for nongraphic characters
      --block-size=SIZE      with -l, scale sizes by SIZE when printing them;
                               e.g., '--block-size=M'; see SIZE format below
  -B, --ignore-backups       do not list implied entries ending with ~
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
  -D, --dired                generate output designed for Emacs' dired mode
  -f                         do not sort, enable -aU, disable -ls --color
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
  -g                         like -l, but do not list owner
      --group-directories-first
tryhackme@linux2:~$
```

## The Man(ual) Page

- we can use the `man` command and then provide the command we want to read the documentation for. 

- Using our `ls` example, we would use man ls to view the manual pages for ls like so:
   
```           
tryhackme@linux2:~$ man ls
LS(1)                                               User Commands                                               LS(1)

NAME
       ls - list directory contents

SYNOPSIS
       ls [OPTION]... [FILE]...

DESCRIPTION
       List  information  about the FILEs (the current directory by default).  Sort entries alphabetically if none of
       -cftuvSUX nor --sort is specified.

       Mandatory arguments to long options are mandatory for short options too.

       -a, --all
              do not ignore entries starting with .

       -A, --almost-all
              do not list implied . and ..

       --author
              with -l, print the author of each file

       -b, --escape
              print C-style escapes for nongraphic characters

       --block-size=SIZE
              with -l, scale sizes by SIZE when printing them; e.g., '--block-size=M'; see SIZE format below

 Manual page ls(1) line 1 (press h for help or q to quit)
 ```
 
 # Answer the questions below
 
 1. What directional arrow key would we use to navigate down the manual page?
 ```
 down
 ```
 2. What flag would we use to display the output in a "human-readable" way?
 ```
 -h
 ```

        






















        
