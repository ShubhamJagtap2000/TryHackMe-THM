# Task 6 - Searching for Files

## Use Find

Take the snippet below, we can see a list of directories available to us:
    
    tryhackme@linux1:~$ ls
    Desktop Documents Pictuers folder1
    tryhackme@linux1:~$

Now, of course, directories can contain even more directories within themselves. 

It becomes a headache when we're having to look through every single one just to try and look for specific files. 

We can use find to do just this for us!

- Let's start simple and assume that we already know the name of the file we're looking for — but can't remember where it is exactly! 

- In this case, we're looking for `"passwords.txt"`

- If we remember the filename, we can simply use `find -name passwords.txt` where the command will look through every folder in our current directory for that specific file like so:

 ```
  tryhackme@linux1:~$ find -name passwords.txt
  ./folder1/passwords.txt
  tryhackme@linux1:~$
 ```
 
`"Find"` has managed to find the file — it turns out it is located in `folder1/passwords.txt — sweet`. 

But let's say that we don't know the name of the file, or want to search for every file that has an extension such as `".txt"`. 

- Find let's us do that too!

- We can simply use what's known as a wildcard (*) to search for anything that has `.txt` at the end. 

- In our case, we want to find every `.txt` file that's in our current directory. 

- We will construct a command such as `find -name *.txt `. 

Where "Find" has been able to find every .txt file and has then given us the location of each one:

    tryhackme@linux1:~$ find -name *.txt
    ./folder1/passwords.txt
    ./Documents/todo.txt
    tryhackme@linux1:~$
    

## Using Grep

Another great utility that is a great one to learn about is the use of `grep`. 

The `grep` command allows us to search the contents of files for specific values that we are looking for.

Take for example the access log of a web server. 

In this case, the `access.log` of a web server has `244` entries.

           
    tryhackme@linux1:~$ wc -l access.log
    244 access.log
    tryhackme@linux1:~$
    
Using a command like cat isn't going to cut it too well here. 

- Let's say for example if we wanted to search this log file to see the things that a certain user/IP address visited? 

- Looking through `244` entries isn't all that efficient considering we want to find a specific value.

- We can use `grep` to search the entire contents of this file for any entries of the value that we are searching for. 

- Going with the example of a web server's access log, we want to see everything that the IP address `"81.143.211.90"` has visited (note that this is fictional)

  ````
  tryhackme@linux1:~$ grep "81.143.211.90" access.log
  81.143.211.90 - - [25/Mar/2021:11:17 + 0000] "GET / HTTP/1.1" 200 417 "-" "Mozilla/5.0 (Linux; Android 7.0; Moto G(4))"
  tryhackme@linux1:~$
  ````
   
- `"Grep"` has searched through this file and has shown us any entries of what we've provided and that is contained within this log file for the IP.


# Answer the questions below

1. Use grep on "access.log" to find the flag that has a prefix of "THM". What is the flag?
```
THM{ACCESS}
```

