# cn_cheatsheet
### some imp qns ahead

### **What is network and network topology?**
What is Network?
A network is a collection of two or more devices connected by communication links so that they can communicate with each other and share resources and information. 

Some examples of networks are email, instant messaging, banking, etc. 

Components of a Network 

• Device: Device means any entity connected to a network and capable of sharing and/or receiving data. It includes devices such as PC, printers, mobile phones, etc. 

• Communication link: A communication channel that connects two devices in a network. The connection can be physical through cables like copper wire, optical fiber or can be wireless like the use of radio waves.    

Reasons for establishing a network: 

Enables easy sharing of resources between network users and processors. 
Provides network users with maximum performance at minimum cost. 
Software and hardware compatibility. 
Centralized management and allocation of network resources. 
Types of Networks 

A computer network can transmit data by two methods- 

1) Point-to-Point: A dedicated communication channel or link connects 2 devices. The two connected devices use the full capacity of the channel as no other devices are connected. 


 2)Multipoint (Broadcast): More than two devices share a single link. Channel capacity is shared between connected devices. 


Network Topology
Abstract

Network topology is the arrangement of nodes and links of a network.
Topologies are categorized as either physical network topology or logical network topology. 
The topology of a network is key to determining its performance. 
Network topology can be categorized into – Bus Topology, Ring Topology, Star Topology, Mesh Topology, Tree Topology.
Scope of Article 

The article gives a basic understanding of what is network topology and what are various types of network topologies and how different topologies affect the performance of the network.

Definition: Network topology tells us about the way the links and nodes/devices are connected i.e., it refers to the layout or arrangement of nodes and links in a computer network. 

Categories of network topology: 

Physical Topology: Describes the placement of various nodes in a computer network. In other words, it shows how network devices are physically connected. 
Logical Topology: Describes the idea of in what way different nodes are connected and how the data is transmitted through the network. So logical topology deals with the data flow in the network. 
Now let us understand why we need network topology. 

Network topology plays a key role while establishing a network, some reasons are: 

Based on the topology used, network performance will be impacted. 
Topology acts as a factor in determining the media type used to cable the network. 
Depending on the topology cost of the network will be affected.  
Types of Network Topologies:
Bus Topology
It is a multipoint connection in which every node/device is connected to a single cable (Backbone cable) via drop lines. 

Bus topology consists of two ends and data is transmitted from one end to another in a single direction i.e., bus topology is unidirectional.  

Terminators are used at the end of the cable so that the electrical signal does not bounce back. 

If the bus topology contains N nodes, then the number of cables required to connect them will be equal to N+1 where N is the number of drop lines and 1 for the backbone cable. 

Advantages: 

Requires a lesser number of cables. 
Easy to install and extend. 
Suitable for temporary and small networks. 
Disadvantages: 

Fault detection is difficult. 
The entire network shuts down if the main cable breaks. 
Limited cable length. 
Transmission speed decreases when more devices are added to the network. 
Low security. 
Ring Topology
In a ring topology, all the nodes are connected to form a ring such that every node will have exactly two neighbors. 

The signal is passed in one direction from one device to another device until it reaches its destination. For the signal to reach from one point to another it must travel through all the intermediate nodes. 

If the ring topology contains N nodes, then the number of cables required to connect them will be equal to N. 

Advantages:

Point-to-point connectivity of the nodes makes it easy to detect and identify faults.
Easy to install.
Cost-effective and inexpensive to install.
Extending or reducing a node from topology is easy as only two links are required to be changed.
The risk of collision is less as only one node is allowed to send data at a time.  
Disadvantages:

If a single node or a transmission line fails, the entire network breaks down.
Communication delay increases as the number of nodes increases.
Less secure.
Star Topology
In star topology, every device in the network is connected to a central device called hub.

All communications are done through the hub i.e. if one device wants to send data to another device, it first has to send data to the hub, and then the hub sends the data to the designated target.

If the star topology contains N nodes, then the number of cables required to connect them will be equal to N. 

Advantages:

Easy to install and modify.
Failure of one node will not affect the entire network.
Easy to detect the failure.
Less cabling is needed.
Disadvantages:

If the central hub breaks down, the whole network collapses.
Too much dependency on the central device.
Mesh Topology
In mesh topology, each device is connected to every other device on the network through a dedicated point-to-point link.

So, if there are N nodes in the network then every single node is connected to N-1 number of nodes. 

If the mesh topology contains N nodes, then the number of cables required to connect them will be equal to N*(N-1)/2. 

Advantages:

No data traffic issues because of the dedicated link between two devices.
Failure of a link or a device doesn’t affect the entire network.
Because of the dedicated point-to-point link, this topology provides high security and privacy.
Easy to identify the fault.
Disadvantages:

The amount of cables required is high.
The cost of implementation and maintenance is high.
Difficult and complicated to install and maintain.
Tree Topology
Tree topology is a combination of star and bus topology. In tree topology, multiple star networks are interconnected with one another using a bus network. This topology consists of a parent-child hierarchy.

Advantages:

 Tree topology allows for the easy addition of nodes and network expansion.
If one segment of the network is down it doesn’t affect the other segments of the network.
Fault detection and correction is easy.
The whole network is divided into segments which makes it easy to manage and maintain.
Disadvantages:

The entire system is dependent on the central hub, if the central hub fails then the entire network fails.
Complex to design and maintain.
Tree topologies are expensive because of cabling.
Summary

Network Topology is the manner in which nodes/devices and links are arranged in a network.
Types of network topologies are –  Bus Topology, Ring Topology, Star Topology, Mesh Topology, Tree Topology.
Every topology has some strengths and weaknesses. So determining the right topology will depend on the needs and size of the network. 
Some of the factors considered while selecting a network topology are reliability, security, cost, and scalability of the topology.
### **Layers of OSI Model**
Layers of OSI Model
The Open System Interconnection (OSI) model is a conceptual model developed by the International Standards Organization (ISO) in 1984. The OSI model provides a standard for communication between different/diverse computer systems.

The OSI model has seven layers in which each layer has a specific set of functions and communicates with the layer above and below itself.

Layers of OSI mode:

Physical Layer: The physical layer is the lowest layer of the OSI model. It is responsible for transmitting message bits over a medium and it also takes care of mechanical, electrical, procedural, and functional specifications for communication.

Functions:
Transmission mode: It defines a transmission mode from Simplex, half-duplex, and full-duplex.
Network Topology: It specifies the arrangement of devices in a network.
Physical characteristics of  the transmission medium
Line Configuration: It selects from either point-to-point or multipoint line configuration.
Data Rate: The physical layer defines the number of bits transmitted per unit of time.
Data Link Layer(DLL): The data link layer breaks data packets received from the network layer into smaller pieces called frames and is responsible for the error-free transmission of these frames from one node to another using its MAC address.

The DLL is divided into two sublayers:
LLC(Logical Link Control): It deals with functions like flow control and error control.
MAC(Media Access Control): It controls the physical addressing and framing functions of the data link layer.
Functions:

Flow Control: It makes sure that the transmitting speed and the amount of data sent match with the capacity and speed of the receiver so that no data gets corrupted.
Framing: DLL adds certain bits at the beginning(called header which contains the source and destination addresses) and at the end(called trailer which contains error correction and detection bits) to the message frame. 
Error Control: DLL uses CRC(cyclic redundancy check) to check if any error occurred during transmission.
Physical Addressing: DLL adds physical address(MAC address) of destination and source in the header of each frame.
Access Control: Determines which device has control over the link if the same communication channel is shared by multiple devices.
### **Define Network**
### **What do you mean by network topology? Explain Types**
### **Define bandwidth, node, and link?**
### **Explain TCP model**
### **OSI Model**
### **What is IP address, private IP address, public IP address?**
### **Different types of delays**
### **What is LAN? Local Area Network**
### **VPN, advantages, and disadvantages of it**
### **Difference between Hub vs Switch**
### **Difference between TCP and UDP**
### **What is the SMTP protocol?**
### **What are HTTP and HTTPS protocols?**
### **RSA Algorithm**
### **3-way handshaking**
### **Difference between IPv4 and IPv6**
### **Significance of Data Link Layer**
### **Define gateway, the difference between gateway and router**
### **What are Firewalls?**
### **Server-side load balancer**
### **What happens when you enter “google.com”?**