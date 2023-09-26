# 🖥️ Net_Practice 🖥️

This repository contains information about networking. <br>
Computers and the internet are a bit like sending letters to friends. <br>
We use addresses, helpers, and special codes to make sure everything goes to the right place. <br>
Routers are like traffic directors to help the letters (data) travel around the neighborhood (the internet) efficiently.

## 🌐 Networking Basics

### 📨 Subnet Mask
A subnet mask is a 32-bit (IPv4) or 128-bit (IPv6) number used to separate the network and host portions of an IP address. <br>
It's represented in decimal (e.g., 255.255.255.0) or CIDR notation (e.g., /24). <br>
In a network, devices or subnets within the same segment often share the same subnet mask. <br>
In larger networks, different subnets with varying subnet masks coexist, interconnected by routers. <br>
Devices in the same subnet have identical network portions in their IP addresses, with the host portion distinguishing individual devices. <br>
The subnet mask defines the number of bits allocated to the network and host portions.

### 📨 Subnet
A subnet is a logical division of an IP network created using a subnet mask. <br>
It consists of a range of IP addresses with a common network address and subnet mask. <br>
Devices in the same subnet can communicate directly without routing. <br>
Subnets improve network organization, security, and efficiency. <br>
Subnets are sssential for IP address management and traffic control <br>
Think of a subnet like a group of friends who live on the same street. They can easily talk to each other because they're in the same group/neigberhoud. <br>

### 📨 Subnet Information

| CIDR Notation | Dotted Decimal Notation | Number of IP Addresses per Subnet | Number of Subnets | Bits  | Binary |
|---------------|-------------------------|-----------------------------------|-------------------|-------|-------------------------------------|
| /32           | 255.255.255.255         | 1                                 | 256               | 32    | 11111111.11111111.11111111.11111111 |
| /31           | 255.255.255.254         | 2                                 | 128               | 31    | 11111111.11111111.11111111.11111110 |
| /30           | 255.255.255.252         | 4                                 | 64                | 30    | 11111111.11111111.11111111.11111100 |
| /29           | 255.255.255.248         | 8                                 | 32                | 29    | 11111111.11111111.11111111.11111000 |
| /28           | 255.255.255.240         | 16                                | 16                | 28    | 11111111.11111111.11111111.11110000 |
| /27           | 255.255.255.224         | 32                                | 8                 | 27    | 11111111.11111111.11111111.11100000 |
| /26           | 255.255.255.192         | 64                                | 4                 | 26    | 11111111.11111111.11111111.11000000 |
| /25           | 255.255.255.128         | 128                               | 2                 | 25    | 11111111.11111111.11111111.10000000 |
| /24           | 255.255.255.0           | 256                               | 1                 | 24    | 11111111.11111111.11111111.00000000 |


### 📨 IP Address
An IP address is a unique numerical label for networked devices to communicate over IP-based networks. <br>
IPv4 uses 32-bit addresses (e.g., 192.168.1.1), while IPv6 uses 128-bit addresses (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334). <br>
They're divided into network and host portions based on the subnet mask. <br>
An IP address is like a phone number for computers. It helps them call each other and send messages over the internet. <br>

### 📨 TCP *(Transmission Control Protocol)*
TCP is a core protocol in the TCP/IP suite. <br>
It provides reliable, connection-oriented communication with data integrity, sequencing, and error detection. <br>
TCP establishes connections, acknowledges data, and retransmits lost packets. <br>
TCP is like a special postman. It makes sure that letters (data) sent between computers arrive in the right order and don't get lost. <br>

### 📨 Routers
Routers connect different IP networks and determine the best data path from source to destination. <br>
Routing tables guide routers in forwarding traffic between subnets or to the internet. <br>
Routers are like traffic directors for the internet. They help data (like packages) find the best way to travel from one computer to another on the internet. <br>

### 📨 Switches
Switches create local area networks (LANs) by forwarding Ethernet frames within a single segment. <br>
Switches are like traffic lights for computers in a neighborhood. They help them talk to each other quickly and without confusion. <br>

### 📨 Routing Table Elements
-  🔵 **Routing Tables** <br>
Essential tools for routers to make forwarding decisions based on destination IP addresses.
Ensure efficient and accurate routing of network traffic.
Think of this like a big list the postman carries, showing all the addresses they know and how to get to them. They use this list to make sure your letters reach the right place.

-  🟢 **Destination Network or IP Address** <br>
Defines the network or specific host to which traffic should be directed.
Represents a range of IP addresses in CIDR notation for networks or a single IP address for hosts.
This is like telling a postman the address of your friend's house so the letter can be delivered to the right place.

-  🔴 **Next-Hop Router or Gateway** <br>
The IP address of the device responsible for forwarding traffic to the final destination.
Can be directly connected to the router or further upstream.
This is like the postman's helper who knows how to get your letter closer to your friend's house. They pass it along until it gets there.

-  🟡 **Subnet Mask *(Netmask)*** <br>
Indicates which part of the IP address is for the network and which is for hosts.
Helps routers determine if an IP address belongs to a specified destination network.
Think of this like the part of the address that says which street your friend's house is on. It helps computers know which group they belong to.

-  🟣 **Interface** <br>
Represents the network interface (e.g., Ethernet, Wi-Fi, VLAN) used to transmit packets to the next-hop router or gateway.
Imagine this as the way the letter or data leaves your house. It's like choosing whether to send a letter through the mailbox or drop it at the post office.

![image]()


## 🌐 Resources

- [Communications and Networks](https://sites.ualberta.ca/dept/chemeng/AIX-43/share/man/info/C/a_doc_lib/aixbman/commadmn/tcp_address.htm#:~:text=TCP%2FIP%20requires%20a%20unique,is%20using%20a%20name%20server.)
- [TCP/IP Explained Simply](https://www.youtube.com/watch?v=tnAW02zvFhU)
- [TCP/IP Protocol Explained](https://www.youtube.com/watch?v=CsektxtqA8c)
- [Configuring a simple network using a router](https://www.youtube.com/watch?v=jhcLWP-SyyE)
- [NetPractice Documentation](https://medium.com/@imyzf/netpractice-2d2b39b6cf0a)
