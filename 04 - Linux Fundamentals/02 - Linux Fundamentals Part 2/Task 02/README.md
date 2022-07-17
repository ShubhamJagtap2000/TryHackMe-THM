# Task 2 - Accessing Your Linux Machine Using SSH (Deploy)

## What is SSH & how Does it Work?

- Secure Shell or SSH simply is a protocol between devices in an encrypted form. 

- Using cryptography, any input we send in a human-readable format is encrypted for travelling over a network -- where it is then unencrypted once it reaches the remote machine, such as in the diagram below.

![Screenshot (753)](https://user-images.githubusercontent.com/63872951/179389370-bdb59db5-753a-4a26-98f8-910aba402dfe.png)

 
- You can learn about the various types of encryption on a TryHackMe room. 

- But for now, we only need to understand that:

    - `SSH` allows us to remotely execute commands on another device remotely.
    - Any data sent between the devices is encrypted when it is sent over a network such as the Internet
    

## Using SSH to Login to Your Linux Machine

The syntax to use SSH is very simple. 

We only need to provide two things:

1. The IP address of the remote machine

2. Correct credentials to a valid account to login with on the remote machine

- The command to do so is ssh and then the `username` of the account, `@` the `IP address` of the machine.

```
ssh tryhackme@MACHINE_IP 
```

