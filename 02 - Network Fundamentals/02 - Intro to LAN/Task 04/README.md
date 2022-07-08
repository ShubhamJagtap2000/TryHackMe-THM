# Task 4 - The DHCP Protocol

- IP addresses can be assigned either manually, by entering them physically into a device, or automatically and most commonly by using a **DHCP** ``(Dynamic Host Configuration Protocol)`` server. 

- When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network. 
 
- The DHCP server then replies back with an IP address the device could use **(DHCP Offer)**. 
- The device then sends a reply confirming it wants the offered IP Address **(DHCP Request)**.

- Then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address **(DHCP ACK)**.

    ![Screenshot (741)](https://user-images.githubusercontent.com/63872951/177950587-740c6a12-4d85-45e0-9d8d-1c12a1e71e5a.png)


# Answer the questions below

1.  What type of DHCP packet is used by a device to retrieve an IP address? 
```
DHCP Discover
```
2.  What type of DHCP packet does a device send once it has been offered an IP address by the DHCP server? 
```
DHCP Request
```
3.  Finally, what is the last DHCP packet that is sent to a device from a DHCP server?
```
DHCP ACK
```
