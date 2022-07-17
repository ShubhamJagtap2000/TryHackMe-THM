# Task 6 - Common Directories

## /etc

- This root directory is one of the most important root directories on your system. 

- The `etc` folder (short for etcetera) is a commonplace location to store system files that are used by your operating system. 

- For example, the sudoers file highlighted in the screenshot below contains a list of the users & groups that have permission to run sudo or a set of commands as the root user.

- Also highlighted below are the `"passwd"` and `"shadow"` files. 
- These two files are special for Linux as they show how your system stores the passwords for each user in encrypted formatting called `sha512`.

```           
tryhackme@linux2:/etc$ ls
shadow passwd sudoers sudoers.d
```

## /var

- The `/var` directory, with `var` being short for variable data,  is one of the main root folders found on a Linux install. 
- This folder stores data that is frequently accessed or written by services or applications running on the system. 

- For example, `log` files from running services and applications are written here `/var/log`, or other data that is not necessarily associated with a specific user (i.e., databases and the like).

```           
tryhackme@linux2:/var$ ls
backups log opt tmp
```

## /root

- Unlike the `/home` directory, the `/root` folder is actually the home for the `root` system user. 

- There isn't anything more to this folder other than just understanding that this is the home directory for the `root` user. 
- But, it is worth a mention as the logical presumption is that this user would have their data in a directory such as `/home/root` by default. 

```        
root@linux2:~# ls
myfile myfolder passwords.xlsx
```

## /tmp

- This is a unique root directory found on a Linux install. 
- Short for `temporary`, the `/tmp` directory is volatile and is used to store data that is only needed to be accessed once or twice. 

- Similar to the memory on your computer, once the computer is restarted, the contents of this folder are cleared out.

- What's useful for us in pentesting is that any user can write to this folder by default. 
- Meaning once we have access to a machine, it serves as a good place to store things like our `enumeration scripts`.

```        
root@linux2:/tmp# ls
todelete trash.txt rubbish.bin
```

# Answer the questions below

1. What is the directory path that would we expect logs to be stored in?
```
/var/log
```

2. What root directory is similar to how RAM on a computer works?
```
/tmp
```

3. Name the home directory of the root user
```
/root
```
