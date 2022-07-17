# Task 5 - Interacting With the Filesystem!

| **Command** |	**Full Name** |
| -- | -- |
| ls | listing |
| cd | change directory |
| cat |	concatenate
| pwd |	print working directory


## Listing Files in Our Current Directory (`ls`)

**Pro tip:** You can list the contents of a directory without having to navigate to it by using ls and the name of the directory. I.e. `ls Pictures`

## Outputting the Contents of a File (`cat`)

- `"Cat"` is short for concatenating & is a fantastic way us to output the contents of files (not just text files!).

**Pro tip:** You can use cat to output the contents of a file within directories without having to navigate to it by using cat and the name of the directory. I.e. `cat /home/ubuntu/Documents/todo.txt`

- Sometimes things like usernames, passwords (yes - really...), flags or configuration settings are stored within files where `"cat"` can be used to retrieve these.

## Finding out the full Path to our Current Working Directory (pwd)

- It's easy to lose track of where we are on the filesystem exactly, which is why I want to introduce `"pwd"`. 
- This stands for **p**rint **w**orking **d**irectory.

# Answer the questions below

1. On the Linux machine that you deploy, how many folders are there? 
```
4
```
2. Which directory contains a file? 
```
folder4
```
3. What is the contents of this file?
```
Hello World
```
4. Use the cd command to navigate to this file and find out the new current working directory. What is the path?
```
/home/tryhackme/folder4
```

