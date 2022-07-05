# Task 1 - Hacking your first machine

Before going into cyber security careers and what offensive security is, let's get you hacking (and yes, its legal, all exercises are fake simulations)

## Your first hack

- Click the ``"Start Machine"`` button. Once loaded, you will have access to a machine you'll use to hack a fake bank application called **FakeBank**.

- We will use a command-line application called ``"GoBuster"`` to **brute-force** FakeBank's website to find hidden directories and pages. 
- GoBuster will take a list of potential page or directory names and tries accessing a website with each of them; if the page exists, it tells you.

## Step 1) Open a Terminal

A terminal, also known as the command-line, allows us to interact with a computer without using a graphical user interface.<br>
On the machine, open the terminal using the Terminal icon.  

## Step 2) Find hidden website pages

Most companies will have an admin portal page, giving their staff access to basic admin controls for day-to-day operations.<br>

For a bank, an employee might need to transfer money to and from client accounts.<br> 

Often these pages are not made private, allowing attackers to find hidden pages that show, or give access to, admin controls or sensitive data.

- Type the following command into the terminal to find potentially hidden pages on FakeBank's website using GoBuster (a command-line security application).

![Screenshot (720)](https://user-images.githubusercontent.com/63872951/177399923-3f9fbb94-6ffe-4d6a-8b6a-acef62b16390.png)

In the command above, `-u` is used to state the website we're scanning, `-w` takes a list of words to iterate through to find hidden pages.

You will see that GoBuster scans the website with each word in the list, finding pages that exist on the site. 

GoBuster will have told you the pages it found in the list of page/directory names (Indicated by Status: 200).

![Screenshot (721)](https://user-images.githubusercontent.com/63872951/177402183-4a8f70b0-78c6-4d67-8a0d-6e7340c44fd5.png)


## Step 3) Hack the bank

You should have found a secret bank transfer page that allows you to transfer money between accounts at the bank (/bank-transfer). 

Type the hidden page into the FakeBank website on the machine.

This page allows an attacker to steal money from any bank account, which is a critical risk for the bank.<br> As an ethical hacker, you would (with permission) find vulnerabilities in their application and report them to the bank to fix before a hacker exploits them.

Transfer $2000 from the bank account 2276, to your account (account number 8881).

# Answer the questions below

 When you've transferred money to your account, go back to your bank account page. What is the answer shown on your bank balance page? 
 ```
 BANK-HACKED
 ```
If you were a penetration tester or security consultant, this is an exercise you’d perform for companies to test for vulnerabilities in their web applications; find hidden pages to investigate for vulnerabilities.
```
No answer needed
```
Terminate the machine by clicking the red "Terminate" button at the top of the page.
```
No answer needed
```
