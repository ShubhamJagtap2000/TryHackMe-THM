# Identifying Devices on a Network

We can change our name through deed poll, but we can't, however, change our fingerprints. 

Every human has an individual set of fingerprints which means that even if they change their name, there is still an identity behind it. 

Devices have the same thing: two means of identification, with one being permeable. 

- These are:

    - An `IP Address`
    
    - A `Media Access Control (MAC) Address` -- think of this as being similar to a serial number.

# IP Addresses

- Briefly, an IP address (or Internet Protocol) address can be used as a way of identifying a host on a network for a period of time, where that IP address can then be associated with another device without the IP address changing. 

- `First`, let's split up precisely what an IP address is in the diagram below:

![Screenshot (725)](https://user-images.githubusercontent.com/63872951/177531294-71829fd8-0fc8-40b8-8e21-0b01b88421bd.png)

- An IP address is a set of numbers that are divided into four octets. 
- The value of each octet will summarise to be the IP address of the device on the network. 
- This number is calculated through a technique known as `IP addressing & subnetting`, but that is for another day. 
- What's important to understand here is that IP addresses can change from device to device but cannot be active simultaneously more than once within the same network.

- IP Addresses follow a set of standards known as `protocols`. 
- These protocols are the backbone of networking and force many devices to communicate in the same language, which is something that we'll come onto another time. 
- However, we should recall that devices can be on both a private and public network. 
- Depending on where they are will determine what type of IP address they have: a `public` or `private IP` address.

- A public address is used to identify the device on the Internet, whereas a private address is used to identify a device amongst other devices. 
- Take the table & screenshot below as an example. Here we have two devices on a private network:

![Screenshot (726)](https://user-images.githubusercontent.com/63872951/177532212-670436bc-7959-4f25-918e-0d98d53ac49d.png)


- These two devices will be able to use their private IP addresses to communicate with each other. 
- However, any data sent to the Internet from either of these devices will be identified by the same public IP address. 

- Public IP addresses are given by your `Internet Service Provider` (or ISP) at a monthly fee (your bill!)

![Screenshot (727)](https://user-images.githubusercontent.com/63872951/177532691-0376d960-866e-4d32-bc56-57de5c6d5133.png)

As more and more devices become connected, it is becoming increasingly harder to get a public address that isn't already in use. 

For example, `Cisco`, an industry giant in the world of networking, estimated that there would be approximately 50 billion devices connected on the Internet by the end of 2021. (Cisco., 2021). 

## Enter IP address versions

So far, we have only discussed one version of the Internet Protocol addressing scheme known as IPv4, which uses a numbering system of `2^32 IP addresses` (4.29 billion).

So you can see why there is such a shortage!

- IPv6 is a new iteration of the Internet Protocol addressing scheme to help tackle this issue. Although it is seemingly more daunting, it boasts a few benefits:

    - Supports up to `2^128 of IP addresses` (340 trillion-plus), resolving the issues faced with IPv4
    
    - More efficient due to new methodologies

The screenshot below compares both an IPv6 and IPv4 address.

![Screenshot (728)](https://user-images.githubusercontent.com/63872951/177533269-272c8f73-8321-481b-8251-5a8e291a7770.png)

# MAC Addresses

Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard. 

This network interface is assigned a unique address at the factory it was built at, called a `MAC (Media Access Control)` address. 

The MAC address is a **twelve-character** **hexadecimal number** (a base sixteen numbering system used in computing to represent numbers) split into two's and separated by a colon. 

These colons are considered separators. 

- For example, `a4:c3:f0:85:ac:2d`. 
- The **first six** characters represent the **company vendor** that made the network interface, and the **last six** is a **unique number**.

![Screenshot (730)](https://user-images.githubusercontent.com/63872951/177534024-0ebc3ea3-91ea-41bd-bf1c-d3d22b994d31.png)


However, an interesting thing with MAC addresses is that they can be faked or "spoofed" in a process known as ``spoofing``. 

This spoofing occurs when a networked device pretends to identify as another using its MAC address. 

When this occurs, it can often break poorly implemented security designs that assume that devices talking on a network are trustworthy. 

- Take the following scenario: ``A firewall`` is configured to allow any communication going to and from the MAC address of the administrator. 
 
- If a device were to pretend or "spoof" this MAC address, the firewall would now think that it is receiving communication from the administrator when it isn't.

- Places such as cafes, coffee shops, and hotels alike often use MAC address control when using their "Guest "or "Public" Wi-Fi. This configuration could offer better services, i.e. a faster connection for a price if you are willing to pay the fee per device.

# Practical Lab
# Answer the questions below

 What does the term "IP" stand for? 
 ```
 Internet Protocol
 ```
 
 What is each section of an IP address called?
 ```
 Octet
 ```
 
 How many sections (in digits) does an IP address have? 
 ```
 4(IPv4)
 ```
 
 What does the term "MAC" stand for?
 ```
 Media Access Control
 ```
 
 

Deploy the interactive lab using the "View Site" button and spoof your MAC address to access the site.  What is the flag?
```
THM{YOU_GOT_ON_TRYHACKME}
```
