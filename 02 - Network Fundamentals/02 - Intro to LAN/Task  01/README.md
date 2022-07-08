# Task 1 - LAN Topologies

Over the years, there has been experimentation and implementation of various network designs.  

In reference to networking, when we refer to the term "topology", we are actually referring to the design or look of the network at hand. 

Let's discuss the advantages and disadvantages of these topologies below.


## 1. Star Topology

The main premise of a star topology is that devices are individually connected via a central networking device such as a switch or hub. 

This topology is the most commonly found today because of its reliability and scalability - despite the cost.

Any information sent to a device in this topology is sent via the central device to which it connects. 

Let's explore some of these advantages and disadvantages of this topology below:

### Advantages

- This topology is much more scalable in nature, which means that it is very easy to add more devices as the demand for the network increases.

### Disadvantages

- Because more cabling & the purchase of dedicated networking equipment is required for this topology, it is more expensive than any of the other topologies.
- The more the network scales, the more maintenance is required to keep the network functional. This increased dependence on maintenance can also make troubleshooting faults much harder.

     ![Screenshot (733)](https://user-images.githubusercontent.com/63872951/177940698-952d1014-e2ed-418a-9d2c-d603ed0688a6.png)

## 2. Bus Topology

This type of connection relies upon a single connection which is known as a backbone cable. 

This type of topology is similar to the leaf off of a tree in the sense that devices (leaves) stem from where the branches are on this cable.

### Disadvantages

- Because all data destined for each device travels along the same cable, it is very quickly prone to becoming slow and bottlenecked if devices within the topology are simultaneously requesting data. 

- This bottleneck also results in very difficult troubleshooting because it quickly becomes difficult to identify which device is experiencing issues with data all travelling along the same route.

- Lastly, ring topologies are less prone to bottlenecks, such as within a bus topology, as large amounts of traffic are not travelling across the network at any one time. The design of this topology does, however, mean that a fault such as cut cable, or broken device will result in the entire networking breaking. 


### Advantages

- However, with this said, bus topologies are one of the easier and more cost-efficient topologies to set up because of their expenses, such as cabling or dedicated networking equipment used to connect these devices.

     ![Screenshot (734)](https://user-images.githubusercontent.com/63872951/177941549-ae241e2e-251a-4013-a483-5048e5779692.png)


## Ring Topology

The ring topology (also known as token topology) boasts some similarities. 

Devices such as computers are connected directly to each other to form a loop, meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology. 

A ring topology works by sending data across the loop until it reaches the destined device, using other devices along the loop to forward the data. 

Interestingly, a device will only send received data from another device in this topology if it does not have any to send itself. 

If the device happens to have data to send, it will send its own data first before sending data from another device.

### Advantages

- Because there is only one direction for data to travel across this topology, it is fairly easy to troubleshoot any faults that arise. 
 
- However, this is a double-edged sword because it isn't an efficient way of data travelling across a network, as it may have to visit many multiple devices first before reaching the intended device.

### Disadvantages

- Lastly, ring topologies are less prone to bottlenecks, such as within a bus topology, as large amounts of traffic are not travelling across the network at any one time. 
 
- The design of this topology does, however, mean that a fault such as cut cable, or broken device will result in the entire networking breaking. 

     ![Screenshot (735)](https://user-images.githubusercontent.com/63872951/177942569-235b0633-6c5a-4d2c-a258-35d460bdfbcd.png)


# What is a Switch?

Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet. 

These various devices plug into a switch's port. 

Switches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network. 

Switches can connect a large number of devices by having ports of 4, 8, 16, 24, 32, and 64 for devices to plug into.

Switches are much more efficient than their lesser counterpart (hubs/repeaters). 

Switches keep track of what device is connected to which port. 

This way, when they receive a packet, instead of repeating that packet to every port like a hub would do, it just sends it to the intended target, thus reducing network traffic.

   ![Screenshot (736)](https://user-images.githubusercontent.com/63872951/177943150-b12164dd-b8e8-4535-958b-e6b6b431790a.png)


- Both Switches and Routers can be connected to one another. 
- The ability to do this increases the redundancy (the reliability) of a network by adding multiple paths for data to take. 
- If one path goes down, another can be used. 

- Whilst this may reduce the overall performance of a network because packets have to take longer to travel, there is no downtime -- a small price to pay considering the alternative.

# What is a Router?

t's a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).

Routing is the label given to the process of data travelling across networks. 

Routing involves creating a path between networks so that this data can be successfully delivered.

Routing is useful when devices are connected by many paths, such as in the example diagram below.

   ![Screenshot (737)](https://user-images.githubusercontent.com/63872951/177943655-7ceb2af8-f1fd-42ab-99bf-e7fdd069364f.png)


# Answer the questions below

1. What does LAN stand for?
```
Local Area Network
```

2. What is the verb given to the job that Routers perform?
```
Routing
```
3. What device is used to centrally connect multiple devices on the local network and transmit data to the correct location?
```
Switch
```
4. What topology is cost-efficient to set up?
```
Bus Topolgy
```
5. What topology is expensive to set up and maintain?
```
Star Topology
```
6. Complete the interactive lab attached to this task. What is the flag given at the end?
```
THM{TOPOLOGY_FLAWS}
```















