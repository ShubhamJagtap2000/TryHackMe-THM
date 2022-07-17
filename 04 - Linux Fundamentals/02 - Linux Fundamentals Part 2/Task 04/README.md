# Task 4 - Filesystem Interaction Contd.

|Command	|Full Name	|Purpose|
|--|--|--|
|touch	|touch	|Create file |
|mkdir	|make directory	|Create a folder|
|cp	|copy	|Copy a file or folder|
|mv	|move	|Move a file or folder|
|rm	|remove	|Remove a file or folder|
|file	|file	|Determine the type of a file|

## Creating Files and Folders(touch, mkdir)

- The `touch` command takes exactly one argument -- the name we want to give the file we create. 

- For example, we can create the file `"note"` by using `touch note`. 

- It's worth noting that `touch` simply creates a blank file. 

- You would need to use commands like echo or text editors such as `nano` to add content to the blank file.

```
tryhackme@linux2:~$ touch note
tryhackme@linux2:~$ ls           
folder1 note
```

- This is a similar process for making a folder, which just involves using the `mkdir` command and again providing the name that we want to assign to the directory. 

- For example, creating the directory `"mydirectory"` using `mkdir mydirectory`.

```           
tryhackme@linux2:~$ mkdir mydirectory
tryhackme@linux2:~$ ls           
folder1 mydirectory note
```

## Removing Files and Folders(rm)

- `rm` is extraordinary out of the commands that we've covered so far. 

- You can simply remove files by using `rm`. 

- However, you need to provide the `-R` switch alongside the name of the directory you wish to remove.

```
tryhackme@linux2:~$ rm note
tryhackme@linux2:~$ ls           
folder1 mydirectory
```

```           
tryhackme@linux2:~$ rm -R mydirectory
tryhackme@linux2:~$ ls           
folder1
```

## Copying and Moving Files and Folders(cp, mv)

- Copying and moving files is an important functionality on a Linux machine. 

- Starting with `cp`, this command takes two arguments:

    1. the name of the existing file

    2. the name we wish to assign to the new file when copying

- `cp` copies the entire contents of the existing file into the new file. 

- In the snippet below, we are copying `"note"` to `"note2"`.

```   
tryhackme@linux2:~$ cp note note2
tryhackme@linux2:~$ ls           
folder1 note note2
```

- Moving a file takes two arguments, just like the `cp` command. 

- However, rather than copying and/or creating a new file, `mv` will merge or modify the second file that we provide as an argument. 

- Not only can you use `mv` to move a file to a new folder, but you can also use `mv` to rename a file or folder. 

- For example, in the snippet below, we are renaming the file `"note2"` to be named `"note3"`. 

- `"note3"` will now have the contents of `"note2"`. 

```
tryhackme@linux2:~$ mv note2 note3
tryhackme@linux2:~$ ls           
folder1 note note3
```

# Determining File Type

- What is often misleading and often catches people out is making presumptions from files as to what their purpose or contents may be. 

- Files usually have what's known as an extension to make this easier. 

- For example, text files usually have an extension of `".txt"`. 

- But this is not necessary.

- So far, the files we have used in our examples haven't had an extension. 

- Without knowing the context of why the file is there -- we don't really know its purpose. 

- Enter the file command. 

- This command takes one argument. 

- For example, we'll use file to confirm whether or not the `"note"` file in our examples is indeed a text file, like so `file note`.

```        
tryhackme@linux2:~$ file note
note: ASCII text
```

# Answer the questions below

1. How would you create the file named "newnote"?
```
touch newnote
```

2. On the deployable machine, what is the file type of "unknown1" in "tryhackme's" home directory? 
```
ASCII text
```

3. How would we move the file "myfile" to the directory "myfolder"  
```
mv myfile myfolder
```

4. What are the contents of this file?
```
THM{FILESYSTEM}
```




              
