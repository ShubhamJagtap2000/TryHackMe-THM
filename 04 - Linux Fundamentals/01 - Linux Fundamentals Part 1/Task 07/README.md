# Task 7 - Intro to Shell Operators

|**Symbol/Operator**	| **Description** |
| -- | -- |
|&|	This operator allows you to run commands in the background of your terminal. |
|&&|	This operator allows you to combine multiple commands together in one line of your terminal. |
|>	|This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere. |
|>>	|This operator does the same function of the `>` operator but appends the output rather than replacing (meaning nothing is overwritten). |


## Operator "&"

- This operator allows us to execute commands in the background. 

- For example, let's say we want to copy a large file. 

- This will obviously take quite a long time and will leave us unable to do anything else until the file successfully copies.

- The `"&"` shell operator allows us to execute a command and have it run in the background (such as this file copy) allowing us to do other things!

## Operator "&&"

- This shell operator is a bit misleading in the sense of how familiar is to its partner `"&"`. 

- Unlike the "&" operator, we can use `"&&"` to make a list of commands to run `for example command1 && command2`. 

- However, it's worth noting that command2 will only run if command1 was successful.

## Operator ">"

- This operator is what's known as an output redirector. 

- What this essentially means is that we take the output from a command we run and send that output to somewhere else.

- A great example of this is redirecting the output of the echo command that we learned in [Task 4](https://tryhackme.com/room/linuxfundamentalspart1). 

- Of course, running something such as `echo howdy` will return "howdy" back to our terminal — that isn't super useful. 

- What we can do instead, is redirect "howdy" to something such as a new file!

- Let's say we wanted to create a file named `"welcome"` with the message `"hey"`. 

- We can run `echo hey > welcome` where we want the file created with the contents "hey" like so:

```
tryhackme@linux1:~$ echo hey > welcome
```
```       
tryhackme@linux1:~$ cat welcome
hey
```

 **Note:** If the file i.e. "welcome" already exists, the contents will be overwritten!
 
 ## Operator ">>"

- This operator is also an output redirector like in the previous operator (>) we discussed. 

- However, what makes this operator different is that rather than overwriting any contents within a file, for example, it instead just puts the output at the end.

- Following on with our previous example where we have the file ``"welcome"`` that has the contents of ``"hey"``. 
The >> operator allows to append the output to the bottom of the file — rather than replacing the contents like so:

- If were to use echo to add ``"hello"`` to the file using the `>` operator, the file will now only have ``"hello"`` and not ``"hey"``.

- The `>>` operator allows to append the output to the bottom of the file — rather than replacing the contents like so:

```
tryhackme@linux1:~$ echo hello >> welcome
```
```       
tryhackme@linux1:~$ cat welcome
hey
hello
```

# Answer the questions below

1. If we wanted to run a command in the background, what operator would we want to use? 
```
&
```
2. If I wanted to replace the contents of a file named "passwords" with the word "password123", what would my command be?
```
echo password123 > passwords
```
3. Now if I wanted to add "tryhackme" to this file named "passwords" but also keep "passwords123", what would my command be?
```
echo tryhackme >> passwords
```
