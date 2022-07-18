# Task 8 - Maintaining Your System: Logs 

We briefly touched upon log files and where they can be found in Linux Fundamentals Part 1. 

However, let's quickly recap. 

Located in the `/var/log` directory, these files and folders contain logging information for applications and services running on your system. 

The Operating System  (OS) has become pretty good at automatically managing these logs in a process that is known as `rotating`.

- I have highlighted some logs from three services running on a Ubuntu machine:

    - An `Apache2` web server
    - Logs for the `fail2ban` service, which is used to monitor attempted brute forces, for example
    - The `UFW` service which is used as a firewall

![Screenshot (775)](https://user-images.githubusercontent.com/63872951/179575496-09eef4ac-7e06-4582-9b75-bf18bf1ab07d.png)


- These services and logs are a great way in monitoring the health of your system and protecting it. 

- Not only that, but the logs for services such as a web server contain information about every single request - allowing developers or administrators to diagnose performance issues or investigate an intruder's activity. 
- For example, the two types of log files below that are of interest:
    
    - access log
    - error log

![Screenshot (776)](https://user-images.githubusercontent.com/63872951/179575725-b28fa2ae-f2bf-4282-a63b-be82545d15a0.png)

There are, of course, logs that store information about how the OS is running itself and actions that are performed by users, such as authentication attempts.

# Answer the questions below

1. What is the IP address of the user who visited the site?
```
10.9.232.111
```

2. What file did they access?
```
catsanddogs.jpg
```
