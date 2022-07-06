# Ping(ICMP)

`Ping` is one of the most fundamental network tools available to us. 

Ping uses `ICMP (Internet Control Message Protocol)` packets to determine the performance of a connection between devices, for example, if the connection exists or is reliable.

The time taken for ICMP packets travelling between devices is measured by ping, such as in the screenshot below. 

This measuring is done using ICMP's echo packet and then ICMP's echo reply from the target device.


Pings can be performed against devices on a network, such as your home network or resources like websites. 

This tool can be easily used and comes installed on Operating Systems (OSs) such as Linux and Windows. 

The syntax to do a simple ping is `ping IP address or website URL`. 

Let's see this in action in the screenshot below.

![Screenshot (731)](https://user-images.githubusercontent.com/63872951/177535713-31cbc2f1-65da-4534-8be7-56f294e4fc7f.png)

- Here we are pinging a device that has the private address of ``192.168.1.254``. 

- **Ping** informs us that we have sent **six ICMP packets**, all of which were received with an average time of <u>5.3 seconds<u>.

  
# Practice Lab
# Answer the following questions
  
 What protocol does ping use? 
 ```
 ICMP 
 ```
 What is the syntax to ping 10.10.10.10?
 ```
 ping 10.10.10.10
 ```
 What flag do you get when you ping 8.8.8.8?
 ```
 THM{I_PINGED_THE_SERVER}
 ```
