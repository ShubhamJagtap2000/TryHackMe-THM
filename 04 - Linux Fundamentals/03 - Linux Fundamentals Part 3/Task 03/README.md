# Task 3 - Terminal Text Editors

Throughout the series so far, we have only stored text in files using a combination of the `echo` command and the `pipe operators (> and >>)`. 
This isn't an efficient way to handle data when you're working with files with multiple lines and the sorts!

## Nano

It is easy to get started with Nano! 

To create or edit a file using `nano`, we simply use `nano filename` -- replacing "filename" with the name of the file you wish to edit.

Once we press enter to execute the command, nano will launch! 

Where we can just begin to start entering or modifying our text. 

You can navigate each line using the "up" and "down" arrow keys or start a new line using the "Enter" key on your keyboard.

![Screenshot (754)](https://user-images.githubusercontent.com/63872951/179531860-3c6dd72b-92a5-4eb8-a6ff-db9a7a4c5301.png)


- Nano has a few features that are easy to remember & covers the most general things you would want out of a text editor, including:

    - Searching for text
    - Copying and Pasting
    - Jumping to a line number
    - Finding out what line number you are on
  
You can use these features of nano by pressing the `Ctrl` key (which is represented as an `^` on Linux)  and a corresponding letter. 

- For example, to exit, we would want to press `Ctrl and X` to exit Nano.

## Vim

VIM is a much more advanced text editor. 

Whilst you're not expected to know all advanced features, it's helpful to mention it for powering up your Linux skills.

- Some of VIM's benefits, albeit taking a much longer time to become familiar with, includes:

    - **Customisable** - you can modify the keyboard shortcuts to be of your choosing
    - **Syntax Highlighting** - this is useful if you are writing or maintaining code, making it a popular choice for software developers
    - VIM works on all terminals where nano may not be installed
    - There are a lot of resources such as [cheatsheets](https://vim.rtorr.com/), tutorials, and the sorts available to you use.

TryHackMe has a [room showcasing VIM](https://tryhackme.com/room/toolboxvim) if you wish to learn more about this editor!

# Answer the questions below

1. Edit "task3" located in "tryhackme"'s home directory using Nano. What is the flag?
```
THM{TEXT_EDITORS}
```
