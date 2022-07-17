# Task 5 - Permissions 101

- Take, for example, the ls command, which lists the contents of the current directory. 

- When using the `-l` switch, we can see ten columns such as in the snippet below. 
- However, we're only interested in the first three columns:

```         
tryhackme@linux2:~$ ls -lh
-rw-r--r-- 1 cmnatic cmnatic 0 Feb 19 10:37 file1
-rw-r--r-- 8 cmnatic cmnatic 0 Feb 19 10:37 file2
```
  
- Although intimidating, these three columns are very important in determining certain characteristics of a file or folder and whether or not we have access to it. 

- A file or folder can have a couple of characteristics that determine both what actions are allowed and what user or group has the ability to perform the given action -- such as the following:

    - Read
    - Write
    - Execute 

- Using `su` to switch to `user2`



```           
tryhackme@linux2:~$ su user2
Password:
user2@linux2:/home/tryhackme$
```

## Briefly: The Differences Between Users & Groups

- The great thing about Linux is that permissions can be so granular, that whilst a user technically owns a file, if the permissions have been set, then a group of users can also have either the same or a different set of permissions to the exact same file without affecting the file owner itself.

- Let's put this into a real-world context; the system user that runs a web server must have permissions to read and write files for an effective web application. 

- However, companies such as web hosting companies will have to want to allow their customers to upload their own files for their website without being the webserver system user -- compromising the security of every other customer. 

- We'll learn the commands necessary to switch between users below.

## Switching Between Users

- Switching between users on a Linux install is easy work thanks to the `su` command. 

- Unless you are the `root` user (or using root permissions through sudo), then you are required to know two things to facilitate this transition of user accounts:

    - The user we wish to switch to
    - The user's password

- The `su` command takes a couple of switches that may be of relevance to you. 
- For example, executing a command once you log in or specifying a specific shell to use. 

- I encourage you to read the `man` page for `su` to find out more. 

- Let's cover the `-l` or `--login` switch.

- Simply, by providing the `-l` switch to `su`, we start a shell that is much more similar to the actual user logging into the system - we inherit a lot more properties of the new user, i.e., environment variables and the likes.

```           
tryhackme@linux2:~$ su user2
Password:
user2@linux2:/home/tryhackme$
```

- For example, when using `su` to switch to `"user2"`, our new session drops us into our previous user's home directory. 
     
```            
tryhackme@linux2:~$ su -l user2
Password:
user2@linux2:~$ pwd
user2@:/home/user2$
```

- Where now, after using `-l`, our new session has dropped us into the home directory of `"user"` automatically. 
        
