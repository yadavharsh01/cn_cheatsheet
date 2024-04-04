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
ayers of OSI mode:
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
A network is a collection of two or more devices connected by communication links so that they can communicate with each other and share resources and information. 

Some examples of networks are email, instant messaging, banking, etc. 

Components of a Network 
Device: Device means any entity connected to a network and capable of sharing and/or receiving data. It includes devices such as PCs, printers, mobile phones, etc. 
Communication link: A communication channel that connects two devices in a network. The connection can be physical through cables like copper wire, and optical fiber or can be wireless like the use of radio waves.    
Reasons for establishing a network: 

Enables easy sharing of resources between network users and processors. 
Provides network users with maximum performance at minimum cost. 
Software and hardware compatibility. 
Centralized management and allocation of network resources. 
Types of Networks 
A computer network can transmit data by two methods- 

Point-to-Point: A dedicated communication channel or link connects 2 devices. The two connected devices use the full capacity of the channel as no other devices are connected.

Multipoint (Broadcast): More than two devices share a single link. Channel capacity is shared between connected devices.

### **What do you mean by network topology? Explain Types**
What do you mean by network topology? Explain Types
Abstract
Network topology is the arrangement of nodes and links of a network.
Topologies are categorized as either physical network topology or logical network topology. 
The topology of a network is key to determining its performance. 
Network topology can be categorized into – Bus Topology, Ring Topology, Star Topology, Mesh Topology, and Tree Topology.
Scope of Article 
The article gives a basic understanding of what is network topology and what are various types of network topologies and how different topologies affect the performance of the network.

Definition:
Network topology tells us about the way the links and nodes/devices are connected i.e., it refers to the layout or arrangement of nodes and links in a computer network. 

Categories of network topology: 
Physical Topology: Describes the placement of various nodes in a computer network. In other words, it shows how network devices are physically connected. 
Logical Topology: Describes the idea of in what way different nodes are connected and how the data is transmitted through the network. So logical topology deals with the data flow in the network. 
Now let us understand why we need network topology. 

Network topology plays a key role while establishing a network, some reasons are: 

Based on the topology used, network performance will be impacted. 
Topology acts as a factor in determining the media type used to cable the network. 
Depending on the topology cost of the network will be affected.  
Types of Network Topologies:
Bus Topology:
It is a multipoint connection in which every node/device is connected to a single cable (Backbone cable) via drop lines. Bus topology consists of two ends and data is transmitted from one end to another in a single direction i.e., bus topology is unidirectional. Terminators are used at the end of the cable so that the electrical signal does not bounce back.


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
Ring Topology:
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
Star Topology:
 In star topology, every device in the network is connected to a central device called a hub.

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
Mesh Topology:
 In a mesh topology, each device is connected to every other device on the network through a dedicated point-to-point link. So, if there are N nodes in the network then every single node is connected to the N-1 number of nodes. 


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
Tree Topology:
Tree topology is a combination of star and bus topology. In tree topology, multiple star networks are interconnected with one another using a bus network. This topology consists of a parent-child hierarchy.


Advantages:
 Tree topology allows for the easy addition of nodes and network expansion.
If one segment of the network is down it doesn’t affect the other segments of the network.
Fault detection and correction are easy.
The wholeṣ network is divided into segments which makes it easy to manage and maintain.
Disadvantages:
The entire system is dependent on the central hub, if the central hub fails then the entire network fails.
Complex to design and maintain.
Tree topologies are expensive because of cabling.
Summary
Network Topology is the manner in which nodes/devices and links are arranged in a network.
Types of network topologies are –  Bus Topology, Ring Topology, Star Topology, Mesh Topology, and Tree Topology.
Every topology has some strengths and weaknesses. So determining the right topology will depend on the needs and size of the network. 
Some of the factors considered while selecting a network topology are reliability, security, cost, and scalability of the topology.
### **Define bandwidth, node, and link?**
A network is a collection of two or more devices connected by communication links so that they can communicate with each other and share resources and information. 

Some important terms related to networks are

Bandwidth:
Network bandwidth is a measure that denotes the maximum capacity of a wired or wireless communication link to transmit data over a network. In other words, we can say that bandwidth measures how much data can be transmitted over a connection link in a given amount of time.

Bandwidth is usually measured in the number of bits, kilobytes, and gigabytes transmitted per second.

Node:
In networking, nodes are connection points inside a network.

A node refers to an entity/device that is connected to a network and is capable of receiving, processing, and/or transmitting data in a network.

A few examples of nodes include computers, printers, modems, bridges, and switches.

Link:
A link refers to the connection or medium by which two devices/nodes are connected in a network. The connection link can either be wired or wireless.

Wired connections are made using cables like an ethernet cable, coaxial cable, optical fibers, etc. 

Wireless connections are made without cables using air as a medium. Infrared, radio, microwave, and satellite are commonly used.
### **Explain TCP model**
Transmission Control Protocol/Internet Protocol(TCP/IP) is a practical network model developed by the Department of Defense (DoD) in the 1960s to support communication between different network devices on the internet. 

TCP is a set of communication protocols that supports network communication.

The TCP model is subdivided into five layers, each containing specific protocols.


Layers of TCP model
Physical Layer
The physical layer translates message bits into signals for transmission on a medium, i.e. the physical layer is the place where the real communication takes place.
Signals are generated depending on the type of media used to connect two devices. For example, electrical signals are generated for copper cables, light signals are generated for optical fibers, and radio waves are generated for air or vacuum.
Physical layer also specifies characteristics like topology(bus,star,hybrid,mesh,ring), line configuration(point-to-point, multipoint) and transmission mode(simplex, half-duplex, full-duplex).
Data Link Layer(DLL)
The DLL is subdivided into 2 layers: MAC(Media Access Control), LLC(Logical Link Control)
The MAC layer is responsible for data encapsulation(Framing) of IP packets from the network layer into frames. Framing means DLL adds a header(which contains the MAC address of source and destination) and a trailer(which contains error-checking data) at the beginning and end of IP packets.
LLC deals with flow control and error control. Flow control: Limits how much data a sender can transfer without overwhelming the receiver. Error Control: Error in the data transmission can be detected by checking the error detection bits in the trailer of the frame.
Network Layer
The network layer adds IP address/logical address to the data segments to form IP packets and finds the best possible path for data delivery. IP addresses are addresses allocated to a device to uniquely identify it on a global scale. Common protocols used in the Network layer are

IP(Internet Protocol): IP uses the receiver’s IP address to determine the best path for the proper delivery of packets to the destination. When a packet is too large to send over a network medium, the sender host’s IP splits it up into smaller fragments. The fragments are reassembled into the original packet on the receiving host. IP is unreliable since it does not ensure delivery or check for errors.
ARP(Address Resolution Protocol): ARP is used to find MAC/physical Addresses from the IP address.
ICMP(Internet Control Message Protocol): ICMP is responsible for error reporting.
Transport Layer 
The transport layer is in charge of flow control (controlling the rate at which data is transferred), end-to-end connectivity, and error-free data transmission. Protocols used in the Transport layer:

TCP(Transmission Control Protocol): 
TCP is a connection-oriented protocol, which means it requires the formation and termination of connections between devices in order to transmit data.
TCP segmentation means that at the sending node, TCP breaks the entire message into segments, assigns a sequence number to each segment, then reassembles the segments into the original message at the receiving end based on the sequence numbers.
TCP is a reliable protocol because it identifies errors and retransmits the damaged frames, and ensures data delivery in the correct order.
UDP(User Datagram Protocol):
UDP is a connectionless protocol, which means it does not require the establishment and termination of connections between devices.
UDP does not support segmentation and lacks error checking and correction which makes it less reliable but more cost-efficient.
Application Layer
This is the uppermost layer, which combines the OSI model’s session, presentation, and application layers. Users can interact with the application and access network resources through this layer.

Protocols used in the Application layer:

HTTP(Hypertext Transfer Protocol): Protocol used to access data on the World Wide Web.
 DNS(Domain Name System): This protocol translates domain names to IP addresses.
SMTP(Simple Mail Transfer Protocol): This protocol is used to send Email messages.
FTP(File Transfer Protocol): This protocol is used to transfer files between computers.
TELNET(Telecommunication Network): It is a two-way communication protocol connecting a local machine to a remote machine.
### **OSI Model**
The Open System Interconnection (OSI) model is a conceptual model developed by the International Standards Organization (ISO) in 1984. The OSI model provides a standard for communication between different/diverse computer systems.

The OSI model has seven layers in which each layer has a specific set of functions and communicates with the layer above and below itself.


Layers of OSI model
Physical Layer:
The physical layer is the lowest layer of the OSI model. It is responsible for transmitting message bits over a medium and it also takes care of mechanical, electrical, procedural, and functional specifications for communication.

Functions:

Transmission mode: It defines a transmission mode from Simplex, half-duplex, and full-duplex.
Network Topology: It specifies the arrangement of devices in a network.
Physical characteristics of the transmission medium
Line Configuration: It selects from either point-to-point or multipoint line configuration.
Data Rate: The physical layer defines the number of bits transmitted per unit of time.
Data Link Layer(DLL):
The data link layer breaks data packets received from the network layer into smaller pieces called frames and is responsible for the error-free transmission of these frames from one node to another using its MAC address.

The DLL is divided into two sublayers:

LLC(Logical Link Control): It deals with functions like flow control and error control.
MAC(Media Access Control): It controls the physical addressing and framing functions of the data link layer.
Functions:

Flow Control: It makes sure that the transmitting speed and the amount of data sent to match the capacity and speed of the receiver so that no data gets corrupted.
Framing: DLL adds certain bits at the beginning(called header which contains the source and destination addresses) and at the end(called trailer which contains error correction and detection bits) to the message frame. 
Error Control: DLL uses CRC(cyclic redundancy check) to check if any error occurred during transmission.
Physical Addressing: DLL adds the physical address(MAC address) of the destination and source in the header of each frame.
Access Control: Determines which device has control over the link if the same communication channel is shared by multiple devices.
Network Layer:
The network layer is responsible for finding the best path for the delivery of data packets from the source host to the destination host. 

Functions:

Host-to-host connectivity.
Fragmentation: The network layer divides the received data into smaller fragments called packets.
Routing: The network layer is responsible for finding the best possible path for a data packet to reach its destination, this is known as routing.
Logical Addressing: The network layer adds the source and destination’s IP address(which is used to identify a device uniquely universally) in the header of the frame.
Transport Layer:
The purpose of the transport layer is to provide a mechanism for the delivery of a message from one to another process and ensure that the data units are delivered sequentially, without error, and without loss or duplication.

Functions

Service Point Addressing: To ensure that the message is sent to the appropriate process the transport layer header includes an address type known as the service point address or port address.
Segmentation and Reassembly: The transport layer receives a message from the session layer, divides it into smaller pieces called segments, and assigns each segment a sequence number that uniquely identifies that segment, and at the destination transport layer reassembles the message based on their sequence numbers.
Flow Control: The transport layer ensures the speed at which data is sent corresponds to the speed at which data is received.
Error Control: The transport layer performs error control to ensure that data reached its destination without any error.
Session Layer:
This is the layer in charge of initiating and terminating communication between the two devices. The session is the period between the start and end of the communication.

Functions

Dialog Control: It means communication between two processes can take place in either a half-duplex or full-duplex way.
Synchronization: The session layer allows adding some checkpoints while transmitting data so that if a failure of some kind occurs between checkpoints, all data can be retransmitted from the most recent checkpoint.
6. Presentation Layer:

The presentation layer converts the information from the application layer into a suitable format for network transmission.

Functions 

Translation: Convert the information sent by the sender into a common format so that it can be understood by the receiver.
Encryption/Decryption: The process of converting an original message into another format for secure transmission is called encryption and obtaining the original message from the encrypted message is called decryption. Key values ​​are used to encrypt and decrypt data.
Compression: Reducing the number of bits in the message to be transmitted.
 Application Layer:
The application layer allows users to access network resources. The application layer is the OSI layer closest to the end-user.

Functions

File transfer, access, and management (FTAM): It allows a user to access, manage and retrieve files on a remote computer.
Mail Services
Directory Services: This layer provides access to global information for various services.
### **What is IP address, private IP address, public IP address?**
IP address
An IP(Internet Protocol) address is a unique address that identifies a computer or device on the internet. It stores information about device location and allows devices to connect with one another as a result. A device or computer must have an address or a unique mechanism by which another device may locate the relevant device for communication to send or receive data, and this is done with the help of an IP address, which distinguishes different computers, routers, or devices on a network.

There are two types of IP address

IPv4: IP version 4(IPv4) is a 32-bit address that contains a set of four numbers each separated from the next by a period(.). Each number in the set can range from 0 to 255.  As a result, the entire IP addressing range is 0.0.0.0 to 255.255.255.255.
IPv6: IP version 6(IPv6) is a 128-bit address that consists of eight groups of four hexadecimal digits, with each group separated by colons(:).An example of an IPv6 address is 2011:0db8:76c5:0000:0000:7bd4:071e:8394.
Classification of IP address

Private IP Address:
Each device on the same network is allocated a unique private IP address, allowing devices on the same internal network to communicate with one another.
As the number of internet-connected devices grows, private IP addresses give an altogether different set of addresses that allow access to a network without taking up public IP address space.
A router assigns private IP addresses to devices so that they can connect to other devices on the same network safely.
Because private addresses are not routed across the Internet and no traffic may be sent to them from the Internet, they provide an extra layer of protection.
  Public IP Address:
The ISP (Internet Service Provider) assigns a public IP address, which is used to access the Internet. A device’s public IP address is used to identify it on the internet and to connect with it outside of the network.

A public IP address can be further classified as

Dynamic IP Address: An IP address that changes from time to time and isn’t always the same is known as a dynamic IP address. Internet Service Providers (ISPs) provide dynamic IP addresses to devices attempting to connect to the internet.
Static IP Address: Static IP addresses are addresses that do not change after they have been assigned to a device. Servers and other key equipment typically utilize static IP addresses.
APIPA

Automatic Private IP Addressing (APIPA) is a feature in operating systems (such as Windows) that enables a computer to automatically assign itself an IP address from the APIPA range when  DHCP(Dynamic Host Configuration Protocol) server is either permanently or temporarily unavailable. APIPA is only valid within a local network segment or subnet.
The Internet Assigned Numbers Authority (IANA) has set aside the range 169.254.0.0-169.254.255.255 for Automatic Private IP Addressing, with a 255.255.0.0 subnet mask.
If a DHCP server becomes available later, the APIPA address is changed to the DHCP server’s address.
To confirm that the specified address is not already in use by another network computer, the client employs Address Resolution Protocol (ARP).
### **Different types of delays**
Types of delay: 
Transmission Delay: Transmission delay is referred to as the time taken to put the data packet onto the outgoing transmission link. Transmission delay depends on the length/size of the packet(L) and bandwidth of the network(B) and is calculated as :
Transmission Delay(Tt) = Data size/bandwidth = (L/B) second
Propagation Delay: The time it takes for the last bit of a data packet to pass across the medium and reach the other end is known as propagation delay. The propagation delay is determined by the distance (D) between the transmitter and receiver, as well as the wave signal’s propagation speed (S). It’s calculated as follows:
 Propagation Delay( Tp )= Distance / Velocity=(D/S)second 
Queuing Delay: When a data packet arrives at its destination, it must queue before being processed. Queuing delay is the amount of time a data packet spends waiting in a queue before being processed. There is no set formula for calculating queuing delay; it is determined by the rate at which incoming packets arrive, the outgoing link’s transmission capacity, and the nature of the network’s traffic. 
Processing Delay: The amount of time it takes processors to process the packet header is known as processing delay. The processing of packets helps in detecting errors and deciding where to route the packet. It doesn’t have a formula because it is determined by the processor’s speed.

### **What is LAN? Local Area Network**
A local Location Network (LAN) is a collection of computers and other devices connected by Ethernet or Wi-Fi within a single, limited area, such as a building, office, or home.

A LAN is a network that is contained inside a small geographic area.  LANs examples are home Wi-Fi networks and small business networks.
The fault tolerance of a LAN is higher, and the network is less congested.
In general, the data transfer rate is high. They range in speed from 100 to 1000 Mbps.
Wired LANs and wireless LANs are the two main forms of LANs.

A wired LAN connects servers and other network devices using switches and Ethernet cables.
Wi-Fi is used to connect devices in a wireless LAN. Wi-Fi is a connection protocol that uses radio waves in the 2.4 GHz and 5 GHz frequencies to connect devices to a LAN.
 Two types of local area network architecture are

 Client-Server: Multiple client devices are connected to a central server on a client-server LAN, which oversees application access, device access, file storage, and network traffic.
 Peer-to-peer: There is no central server in a peer-to-peer LAN, and each device contributes equally to the network’s operation. Peer-to-peer LANs are usually smaller and can’t manage a lot of traffic.
### **VPN, advantages, and disadvantages of it**
A Virtual Private Network (VPN) is a secure encrypted connection that ensures sensitive data is delivered securely and privately through a less-secure network, such as the Internet.

By allowing the network to route your IP address through a VPN host’s specially configured distant server, a VPN hides your IP address. Using a VPN makes it harder for third parties to track users’ online activities and steal data, ensuring security, privacy, and anonymity for users.

Advantages
VPN provides secure connections with encrypted data: It helps to protect the personal information that is transmitted and received by the device. 
VPN Hides Your Online Identity: VPN can hide a user’s IP address and browsing history.
 VPNs Help You Bypass geo-blocks: Because some web content is only available in specific parts of the world, utilizing a VPN might make it appear as if you are accessing the internet from a location that is acceptable to the service you are attempting to access.
 VPNs are scalable, which means we can add new locations to the VPN easily. 
VPN protects from Cyberattacks.
 VPN security is cost-effective.
Disadvantages
Internet connections may be slowed by using a VPN.
 VPNs do not provide complete protection against all threats.
 A VPN may not be supported by all devices.
 Dropped Connection: The VPN may occasionally drop the connection and cause you to lose access to the internet. Data leaks can occur as a result of dropped connections, compromising the user’s security, privacy, and anonymity. 
In some countries, using a VPN is illegal.
 It’s difficult to set up a VPN. 
Using the Wrong VPN can risk your privacy.
### **Difference between Hub vs Switch**
                              HUB	                        SWITCH
A hub is a networking device that allows multiple devices to connect to a single network..	A switch is a networking device that connects various devices on a single network.
Hub is a physical layer device, which means it operates at OSI model layer 1.	A switch is a data link layer device, which means it operates at OSI model layer 2.
Hub is a passive Device (Without Software)	A switch is a networking and active device (with software).
Hub uses broadcast-type transmission.	The switch uses unicast, multicast as well as broadcast-type transmission.
Half-duplex communication is supported by a Hub, which means that only one device can send or receive data at a time.	Full-duplex mode is supported by the switch, which means both devices can send and receive data at the same time.
Hub has 4/12 ports.	A switch can have 24 to 48 ports.
There is only one collision domain in Hub.	Each port in Switch has its collision domain.
A network hub cannot learn or store a MAC address.	Switches use content-accessible memory CAM tables.
Hub does not provide packet filtering.	A switch provides packet filtering.
Hub is not an intelligent device as it sends the message to all ports.	A switch is an intelligent device as it sends the message only to the desired destination.
For data transmission, the hub uses electrical signals or bits.	For data transmission, a switch uses frames and packets.
Hub speed is up to 10 Mbps	Switch speed is up to 10/100 Mbps, 1 Gbps.
### **Difference between TCP and UDP**
Feature	                        TCP	                        UDP
Acronym for	Transmission Control Protocol	User Datagram Protocol.
Connection Type	TCP is a connection-oriented protocol, which means it requires the establishment of a connection to transfer data and the termination of that connection once the data has been transmitted.	UDP is a connectionless protocol, which means it doesn’t require establishing, maintaining, or terminating a connection to send data.
Segmentation	TCP allows segmentation, breaking the entire message into segments, assigning a sequence number to each segment, and then reassembling the segments into the original message based on the sequence numbers at the receiving end.	UDP does not support segmentation. In UDP, there is no data sequencing. If sequencing is required, it has to be managed by the application layer.
Reliability 	TCP is reliable as it guarantees data delivery to the destination router.	UDP is unreliable as it does not guarantee the delivery of data to the destination.
Error checking	TCP  provides error-checking mechanisms and also makes error recovery.	UDP follows basic mechanisms of data checking like checksums.
Retransmission	In TCP, if a data packet is lost, it is possible to retransmit the lost packet.	It is not possible to retransmit a lost data packet in UDP.
Speed	TCP is slower than UDP.	UDP is faster than TCP.
Acknowledgment	In TCP, an acknowledgment segment is present.	UDP has no acknowledgment segments.
Header Length	TCP uses a variable-length (20-60) bytes header.	UDP has a fixed-length header of 8 bytes.
Flow Control	TCP uses a flow control technique to ensure that no more than a certain number of data packets are sent to the receiver at the same time.	The UDP protocol has no such mechanism.
Broadcasting	TCP does not support broadcasting.	UDP supports broadcasting.
Handshake	SYN-ACK, SYN, and ACK protocols are used by TCP to establish connections.	UDP does not need any handshake protocol because it is a connectionless protocol.
Optimal Use	TCP is used by HTTPS, HTTP, SMTP, POP, FTP, etc	The UDP protocol is used by DNS, VoIP, media streaming, video conferencing systems, and other applications.
### **What is the SMTP protocol?**
The Simple Mail Transfer Protocol (SMTP) is an application layer protocol that allows the software to send electronic mail over the internet efficiently and reliably.
SMTP is based on a client-server model and uses TCP/IP for sending and receiving mails.
The original standard port for SMTP is Port 25.
An email is made up of two parts: a header and a body, both of which are separated by a null line. The real information to be read by the receiver is contained in the body. The header mostly comprises the topic of the email and the sender’s and recipient’s addresses.
SMTP requires a 7-bit ASCII format for all messages.
Working
The user-agent (UA) and mail transfer agent (MTA) are two components of the SMTP client and SMTP server. The user agent (UA) prepares the message, generates the envelope, inserts the message into it and MTA transfers the mail across the internet.
The client who wishes to send an email establishes a TCP connection with the SMTP server, which is always listening. The SMTP server initiates a connection to that port as soon as it listens for one. The client process sends the email immediately after successfully establishing a TCP connection. The mail is then transferred from the sender’s mail server to the recipient’s mail server using SMTP. Another protocol is required to retrieve mail from the receiver’s mail server to the receiver (commonly POP and IMAP)
When sending an email, SMTP is used twice: first to send the email from the sender to the sender’s mail server, and again to send the email from the sender’s mail server to the receiver’s mail server.

### **What are HTTP and HTTPS protocols?**
HyperText Transfer Protocol(HTTP) is an application layer protocol that is used to access and transfer data(text, images, video, multimedia, etc) over the world wide web.
 HTTP is a client-server protocol that runs on top of the TCP/IP family of protocols and uses the request/response protocol.
HTTP uses port number 80. 
In HTTP, the client sends a request message to the server. After the client responds, HTTP establishes a TCP connection between the client and the server. HTTP delivers a request to the server, which collects the data that was requested. After the server sends data to the client, the connection will be terminated.
 If we want something else from the server, we should have to re-establish the connection between client and server.
Features of HTTP
HTTP is connectionless: After serving a single HTTP request, the client-server connection is closed and that same connection is never used again.
HTTP is media independent: It means that HTTP can send any sort of data as long as both the client and the server understand how to process the data.
HTTP is stateless: The client and server only know about each other during the current request, and when the connection is disconnected, both the client and the server forget about each other.
HTTPS
Hypertext Transfer Protocol Secure is a secure extension or version of HTTP that is used for providing security to the data sent over the world wide web.

This protocol allows transferring the data in an encrypted form which is particularly important when users transmit sensitive data such as login credentials.

To encrypt communications HTTPS uses an encryption protocol called Transport Layer Security (TLS), formerly known as Secure Sockets Layer (SSL). 

HTTPS protocol uses the 443 port number for communicating the data.
### **RSA Algorithm**
The RSA algorithm, developed by Rivest, Shamir, and Adleman in 1978, is an asymmetric cryptography algorithm for encrypting and decrypting messages.
Asymmetric means that the sender and receiver use two different keys for encryption and decryption: a private key and a public key.
The public key is shared openly and is thus known to everyone, whereas the private key is kept secret and is not shared.
The sender encrypts the data to be sent with the receiver’s public key and the receiver decrypts the encrypted message using its private key.

Steps in RSA algorithm

1. Generating the keys:

Select two different large random prime numbers, p and q.
Calculate n=p*q where n is the modulus for the public key and the private keys.
Calculate the totient function; ϕ(n)=(x−1)(y−1).
Select an integer e such that 1<e<ɸ(n) and e is co-prime to ɸ(n),gcd(e,ɸ(n))=1.
Calculate d such that e.d=1 mod ϕ(n).
 Public key is  given as <e,n> and private key as <d,n>.
2. Encryption:

The ciphertext C obtained from plain text P using the public key< e,n> is as follows:

C = Pe mod n
3. Decryption:

The Plaintext P obtained from CipherText C using the private key <d,n> is as follows:

P = Cd  mod n.
### **3-way handshaking**
A three-way handshake is a 3 step process that TCP/IP networks use to establish a secure and reliable connection between sender(client) and receiver(server).

A three-way handshake includes the following steps:

Step 1(SYN):
  To establish a connection, the client sends an SYN (Synchronize Sequence Number) request to the server.
 The request message contains information like the initial sequence number, maximum segment size,  window size, SYN bit set to 1, and ACK bit set to 0. 
The client then awaits a response from the server.
Step 2(SYN+ACK):
  The server answers with an SYN-ACK message after receiving the client’s request.
In the response, both ACK and SYN  bits are set to 1 indicating the server has acknowledged the request and wishes to establish a connection with the client.
The server also sends a random sequence number, window size, maximum segment size, and ACK’s acknowledgment number(which is the client’s received sequence number+1).
Step 3(ACK):  
The client sends an acknowledgment(ACK) to the server after receiving SYN-ACK from the server.
 The client sets the ACK bit to 1 and sends it to the server along with an acknowledgment number (which is the server’s SYN sequence number +1) and also sets the SYN bit to 0.
After this procedure is completed, the client and server establish a connection through which they will begin the data transfer.

### **Difference between IPv4 and IPv6**
Difference between IPv4 and IPv6
        IPv4	    vs               IPv6
Internet protocol version 4 is a 32-bit IP address.	Internet protocol version 4 is a 128-bit IP address.
The address space of the IPv4 address is 4.29 ×10^9.	The address space of the IPv6 address is  3.4 x 10^38.
IPv4 is represented in decimal format.	IPv6 is represented in hexadecimal format.
IPv4 consists of 4 octets where each octet ranges from 0 to 255 and is separated by period(.).	IPv6  consists of 8 groups of 4 hexadecimal digits each group separated by a colon(:).
IPv4 header is 20-60 bytes.	The IPv6 header is fixed at 40 bytes.
The transmission scheme in IPv4 is broadcasting.	The transmission scheme in IPv6 is multicast and anycasting.
IPv4 supports VLSM(variable length subnet mask)	IPv6 does not support VLSM.
IPv4 supports DHCP and manual address configuration.	IPv6 supports autoconfiguration and renumbering configuration.
In IPv4 fragmentation is done by sending and forwarding routes.	In IPv6 fragmentation is done only by the sender.
In IPv4 checksum field is available.	In IPv6 checksum field is not available.
Encryption and authentication are not provided in IPv4.	Encryption and authentication are provided in IPv6.
IPv4 uses ARP(Address Resolution Protocol) to map to MAC addresses.	IPv6 uses NDP(Neighbor Discovery Protocol) to map to the MAC address.

### **Significance of Data Link Layer**
Data Link Layer(DLL):
The data link layer breaks data packets received from the network layer into smaller pieces called frames and is responsible for the error-free transmission of these frames from one node to another using its MAC address.

The DLL is divided into two sublayers:

LLC(Logical Link Control): It deals with functions like flow control and error control.
MAC(Media Access Control): It controls the physical addressing and framing functions of the data link layer.
Functions
Flow Control: It makes sure that the transmitting speed and the amount of data sent to match the capacity and speed of the receiver so that no data gets corrupted.
Framing: DLL adds certain bits at the beginning(called header which contains the source and destination addresses) and at the end(called trailer which contains error correction and detection bits) to the message frame. 
Error Control: DLL uses CRC(cyclic redundancy check) to check if any error occurred during transmission.
Physical Addressing: DLL adds the physical address(MAC address) of the destination and source in the header of each frame.
Access Control: Determines which device has control over the link if the same communication channel is shared by multiple devices.
Significance of data link layer
The data link layer is in charge of delivering data between two network nodes that are directly connected.
The data link layer uses a physical address for the unique identification of each device on a local network.
The data link layer splits packets from the network layer into smaller units known as frames and adds a header(which contains the physical address of source and destination) and a trailer(which contains error-checking data) at the beginning and end of the frame.
Damaged or lost frames are detected and retransmitted by the data link layer’s error control mechanism.
 If many devices share the same communication link, the data link layer determines which device has control over the link.
The data link layer also ensures flow control by limiting the amount of data a transmitter can send without overwhelming the receiver.
Note:

The data link layer is responsible for transmission, flow control, and error control between two nodes, whereas the transport layer is responsible for inter-network flow control and error control.
### **Define gateway, the difference between gateway and router**
A gateway is a network node that serves as an entry and exit point for a network connecting two networks with different sets of protocols, as well as converting one protocol into the other.

Difference between gateway and router

                            Gateway	vs                            Router
A device that acts as a gate and connects two networks having different sets of protocols.	A networking device that manages and forwards data packets to computer networks.
The main principle of a gateway is to convert one protocol to the other.	The main principle of the router is to route traffic from one network to another with the best route.
A gateway acts as a connection between two dissimilar networks.	A router transports data packets over similar networks.
A gateway does not support dynamic routing.	A router supports dynamic routing.
A gateway can operate until layer 5 of the OSI model.	A router can operate only on layer 3 and layer 4 of the OSI model.
### **What are Firewalls?**
Firewall – A firewall is a network security device that monitors incoming and outgoing network traffic and permits or blocks data packets based on a set of security rules. Its purpose is to establish a barrier between your internal network and incoming traffic from external sources (such as the internet) in order to block malicious traffic like viruses and hackers.

How do Firewalls Work :
Firewalls carefully analyze incoming traffic based on pre-established rules and filter traffic coming from unsecured or suspicious sources to prevent attacks. Firewalls guard traffic at a computer’s entry point called ports, which is where information is exchanged with external devices. For example, “Source address 172.18.1.1 is allowed to reach destination 172.18.2.1 over port 22.”

Think of IP addresses as houses, and port numbers as rooms within the house. Only trusted people (source addresses) are allowed to enter the house (destination address) at all—then it’s further filtered so that people within the house are only allowed to access certain rooms (destination ports), depending on if they’re the owner, a child, or a guest. The owner is allowed into any room (any port), while children and guests are allowed into a certain set of rooms (specific ports).

Types of Firewalls :
Firewalls can either be software or hardware, though it’s best to have both. A software firewall is a program installed on each computer and regulates traffic through port numbers and applications, while a physical firewall is a piece of equipment installed between your network and gateway.

Packet-filtering firewalls, the most common type of firewall, examine packets and prohibit them from passing through if they don’t match an established security rule set. This type of firewall checks the packet’s source and destination IP addresses. If packets match those of an “allowed” rule on the firewall, then it is trusted to enter the network.

Packet-filtering firewalls are divided into two categories: stateful and stateless. Stateless firewalls examine packets independently of one another and lack context, making them easy targets for hackers. In contrast, stateful firewalls remember information about previously passed packets and are considered much more secure.

While packet-filtering firewalls can be effective, they ultimately provide very basic protection and can be very limited—for example, they can’t determine if the contents of the request that’s being sent will adversely affect the application it’s reaching. If a malicious request that was allowed from a trusted source address would result in, say, the deletion of a database, the firewall would have no way of knowing that. Next-generation firewalls and proxy firewalls are more equipped to detect such threats.

Next-generation firewalls (NGFW) 
Next-generation firewalls (NGFW) combine traditional firewall technology with additional functionality, such as encrypted traffic inspection, intrusion prevention systems, anti-virus, and more. Most notably, it includes deep packet inspection (DPI). While basic firewalls only look at packet headers, deep packet inspection examines the data within the packet itself, enabling users to more effectively identify, categorize, or stop packets with malicious data. 

Proxy firewalls
Proxy firewalls filter network traffic at the application level. Unlike basic firewalls, the proxy acts as an intermediary between two end systems. The client must send a request to the firewall, where it is then evaluated against a set of security rules and then permitted or blocked. Most notably, proxy firewalls monitor traffic for layer 7 protocols such as HTTP and FTP and use both stateful and deep packet inspection to detect malicious traffic.

Network address translation (NAT)
Network address translation (NAT) firewalls allow multiple devices with independent network addresses to connect to the internet using a single IP address, keeping individual IP addresses hidden. As a result, attackers scanning a network for IP addresses can’t capture specific details, providing greater security against attacks. NAT firewalls are similar to proxy firewalls in that they act as an intermediary between a group of computers and outside traffic.

Stateful multilayer inspection (SMLI)
Stateful multilayer inspection (SMLI) firewalls to filter packets at the network, transport, and application layers, comparing them against known trusted packets. Like NGFW firewalls, SMLI also examines the entire packet and only allows them to pass if they pass each layer individually. These firewalls examine packets to determine the state of the communication (thus the name) to ensure all initiated communication is only taking place with trusted sources.

Why Firewall?
Firewalls are primarily used to prevent malware and network-based attacks. Additionally, they can help in blocking application-layer attacks. These firewalls act as a gatekeeper or a barrier. They monitor every attempt between our computer and another network. They do not allow data packets to be transferred through them unless the data is coming or going from a user-specified trusted source.

Firewalls are designed in such a way that they can react quickly to detect and counter-attacks throughout the network. They can work with rules configured to protect the network and perform quick assessments to find any suspicious activity. In short, we can point to the firewall as a traffic controller.

Some of the important risks of not having a firewall are:

Open Access
If a computer is running without a firewall, it is giving open access to other networks. This means that it is accepting every kind of connection that comes through someone. In this case, it is not possible to detect threats or attacks coming through our network. Without a firewall, we make our devices vulnerable to malicious users and other unwanted sources.

Lost or Comprised Data
Without a firewall, we are leaving our devices accessible to everyone. This means that anyone can access our device and have complete control over it, including the network. In this case, cybercriminals can easily delete our data or use our personal information for their benefit.

Network Crashes
In the absence of a firewall, anyone could access our network and shut it down. It may lead us to invest our valuable time and money to get our network working again.

Therefore, it is essential to use firewalls and keep our network, computer, and data safe and secure from unwanted sources.

Limitations of Firewall:
The importance of using firewalls as a security system is obvious; however, firewalls have some limitations:

Firewalls cannot stop users from accessing malicious websites, making them vulnerable to internal threats or attacks.
Firewalls cannot protect against the transfer of virus-infected files or software.
Firewalls cannot prevent the misuse of passwords.
Firewalls cannot protect if security rules are misconfigured.
Firewalls cannot protect against non-technical security risks, such as social engineering.
Firewalls cannot stop or prevent attackers with modems from dialing in to or out of the internal network.
Firewalls cannot secure the system which is already infected.
Summary
A firewall can be defined as a special type of network security device or a software program that monitors and filters incoming and outgoing network traffic based on a defined set of security rules. It acts as a barrier between internal private networks and external sources (such as the public Internet).
The primary purpose of a firewall is to allow non-threatening traffic and prevent malicious or unwanted data traffic to protect the computer from viruses and attacks. A firewall is a cybersecurity tool that filters network traffic and helps users block malicious software from accessing the Internet on infected computers.
Although Firewalls are important, they have some limitations as well.
### **Server-side load balancer**
Load balancing refers to efficiently distributing the incoming network traffic across a group of backend servers
Load Balancing is of Two Types 
Server Side load balancing 
Client Side Load Balancing
Scope of the Article
This article covers the basic definition of Load Balancing and explains the Server Side Load Balancing along with some consequences to keep in mind when using Server Side Load Balancing and its advantages.

Definition
In Server-side load balancing, the instances of the service are deployed on multiple servers and then a load balancer is put in front of them. It is generally a hardware load balancer. All the incoming requests traffic firstly comes to this load balancer acting as a middle component. It then decides to which server a particular request must be directed based on some algorithm.

We could understand it in this way – It accepts incoming network, and application traffic, and distributes the traffic across the multiple backend servers by using various methods. The middle component is responsible for distributing the client requests to the server.


How Does Server Load Balancing Work?
Server load balancing works within two main types of load balancing:

Transport-level load balancing is a DNS-based approach that acts independently of the application payload.
Application-level load balancing uses traffic load to make balancing decisions such as with windows server load balancing.
Advantages of Server Load Balancing
Distributing incoming network traffic through web server load balancers across multiple servers aims to increase the efficiency of application delivery to end users for a reliable application experience. IT teams are increasingly relying on server load balancers to:

Increase Scalability: load balancers are able to spin up or down server resources based on spikes in traffic to the pool of servers that are best suited to handle these increases in traffic and keep applications’ performance optimized.
Redundancy: Using multiple web servers to deliver applications or websites provides a safeguard against the inevitable hardware failure and application downtime. When server load balancers are in place they can automatically transfer traffic to working servers from servers that go down with little to no impact on the end user.
Maintenance and Performance: Businesses with web servers distributed across multiple locations and a variety of cloud environments can schedule maintenance at any time to improve performance with minimal impact on application uptime as server load balancers can redirect traffic to resources that are not undergoing maintenance.
Some Consequences of using Server Side Load Balancing
The server-side load balancer acts as a single point of failure if it fails, all the instances of the microservice become inaccessible as only the load balancer has the list of servers.
Since each microservice will have a separate load balancer, the overall complexity of the system increases and it becomes hard to manage.
The network latency increases as the number of hops for the request increases from one to two with the load balancer, one to the load balancer, and then another from the load balancer to the microservice.
Summary 
Server Load Balancing (SLB) is a technology that distributes high-traffic sites among several servers using network-based hardware or software-defined appliance.
The servers can be on-premises in a company’s own data centers or hosted in a private cloud or the public cloud.
Server load balancing distributes client traffic to servers to ensure consistent, high-performance application delivery.
Server load balancing ensures application delivery, scalability, reliability, and high availability.
### **What happens when you enter “google.com”?**
Pre – Requisites 

What is a WebPage  -> Before getting started, I want to first explain what a webpage is. A webpage is basically a text file formatted a certain way so that your browser (ie. Chrome, Firefox, Safari, etc) can understand it; this format is called HyperText Markup Language (HTML). These files are located in computers that provide the service of storing said files and waiting for someone to need them to deliver them. They are called servers because they serve the content that they hold to whoever needs it.
Servers -> These servers can vary in classes, the most common and the one that we’ll be talking about in the main portion of this article is a web server, the one that serves web pages. We can also find application servers, which are the ones that hold an application base code that will then be used to interact with a web browser or other applications. Database servers are also out there, which are the ones that hold a database that can be updated and consulted when needed.
IP Addresses -> These servers in order to deliver their content, much like in physical courier services, need to have an address so that the person needing to be said content can make a “letter” requesting the delivery; the person requesting the content in turn also has an address where the server can deliver the content to. These addresses are called IP (Internet Protocol) Addresses, a set of 4 numbers that range from 0 to 255 (one byte) separated by periods (ie. 127.0.0.1).
Protocols for Delivery -> Another concept that is important to know is that the courier service traffic for the delivery can be one of two: Transmission Control Protocol (TCP) and User Datagram Protocol (UDP). Each one determines the way the content of a server is served or delivered.
4.1 TCP -> TCP is usually used to deliver static websites such as Wikipedia or Google and also email services and to download files to your computer because TCP makes sure that all the content that is needed gets delivered. It accomplishes this by sending the file in small packets of data and along with each packet a confirmation to know that the packet was delivered; that’s why if you are ever downloading something and your internet connection suddenly drops when it comes back up you don’t have to start over because the server would know exactly how many packets you have and how many you still need to receive. The downside to TCP is that because it has to confirm whether you got the packet or not before sending the next, it tends to be slower.

4.2 UDP-> UDP, on the other hand, is usually used to serve live videos or online games. This is because UDP is a lot faster than TCP since UDP does not check if the information was received or not; it is not important. The only thing UDP cares about is sending the information. That is the reason why if you’ve ever watched a live video and if either your internet connection or the host’s drops, you would just stop seeing the content; and when the connection comes back up you will only see the current stream of the broadcast and what was missed is forever lost. This is also true for online videogames (if you’ve played them you know exactly what this means)

What Actually happens….

So back to the main question of what happens when you type www.google.com or any other URL (Uniform Resource Locator) in your web browser and press Enter. 

So the first thing that happens is that your browser looks up in its cache to see if that website was visited before and the IP address is known. 
If it can’t find the IP address for the URL requested then it asks your operating system to locate the website. The first place your operating system is going to check for the address of the URL you specified is in the host file. If the URL is not found inside this file, then the OS will make a DNS request to find the IP Address of the web page.
The first step is to ask the Resolver (or Internet Service Provider) server to look up its cache to see if it knows the IP Address, if the Resolver does not know then it asks the root server to ask the .COM TLD (Top Level Domain) server – if your URL ends in .net then the TLD server would be .NET and so on – the TLD server will again check in its cache to see if the requested IP Address is there. 
If not, then it will have at least one of the authoritative name servers associated with that URL, and after going to the Name Server, it will return the IP Address associated with your URL. All this was done in a matter of milliseconds WOW!
After the OS has the IP Address and gives it to the browser, it then makes a GET (a type of HTTP Method) to said IP Address. When the request is made the browser again makes the request to the OS which then, in turn, packs the request in the TCP traffic protocol we discussed earlier, and it is sent to the IP Address. 
On its way, it is checked by both the OS’ and the server’s firewall to make sure that there are no security violations. And upon receiving the request the server (usually a load balancer that directs traffic to all available servers for that website) sends a response with the IP Address of the chosen server along with the SSL (Secure Sockets Layer) certificate to initiate a secure session (HTTPS). 
Finally, the chosen server then sends the HTML, CSS, and Javascript files (If any) back to the OS who in turn gives it to the browser to interpret it. And then you get your website as you know it.
Summary
In our modern society when everything is online, it is amazing to know the complexity that takes place in order for us to be able to get to a website. Yet, it is done so fast that very few would even begin to fathom the amazing process that takes place.

I hope this brief article has given you more insight into everything that happens “under the hood” when you type www.google.com in your browser and hit Enter.