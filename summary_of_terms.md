### **IP ADDRESS**

An IP address is a unique identifier that each device on a network must have for communication purposes. There are two versions of an IP address called IPv4 and IPv6. An IPv4 address is a 32-bit numeric address written as four number separated by a period. Each number separated by a period represents an octet, so in total there are 4 octets in IPv4 address. An octet in IPv4 can be a number from 0 to 255.

There are two parts in an IP address, the first part is for the network address and the second for the host address. The network address is a number that’s assigned to a network, so every network will have a unique address. The host address is a number that is assigned to a host within that network i.e., each host within a network will have a unique host address. 

### **SUBNETS**

A subnet, or subnetwork, is a network inside a network. Subnets make networks more efficient. Through subnetting, network traffic can travel a shorter distance without passing through unnecessary routers to reach its destination.

Because an IP address is limited to indicating the network and the device address, IP addresses cannot be used to indicate which subnet an IP packet should go to. Routers within a network use something called a subnet mask to sort data into subnetworks.

### **SUBNET MASK**

Subnet mask is a number that resembles an IP address and reveals how many bits in the IP address are used for the network by masking the network portion of the IP address. It is a way to divide an IP address into subnets and specify the network’s available hosts. Routers use subnet masks to route data packets to the right subnet.

### **CDIR NOTATION**

It is a shorter way to write a subnets mask and it does this by adding a forward slash and a number to an IP address; the number represents the length of the subnets mask and the number of 1s in it, which are significant in routing. For example, in 192.168.3.0/24 the subnet mask is 24 bits in length and has 24 1s in it.

### **IP ROUTING**

IP Routing is an umbrella term for the set of protocols that determine the path that data follows to travel across multiple networks from its source to its destination. Data is routed from its source to its destination through a series of routers, and across multiple networks. 

Routers refer to internal routing tables to make decisions about how to route packets along network paths. A routing table records the paths that packets should take to reach every destination that the router is responsible for. When a router receives a packet, it reads the header of the packet to see its intended destination, then it determines where to route the packet based on information in its routing tables.

Routing tables can be static or dynamic. Static routing table do not change unless you change them manually whereas dynamic routing tables update automatically. Dynamic routing uses various protocols to determine the shortest and fastest paths, so they require more computing power than static routing tables. The main IP routing protocols are IP, BGP, OSFP and RIP.

### **INTERNET GATEWAY**

An Internet gateway is a network "node" that connects two different networks that use different protocols (rules) for communicating. In the most basic terms, an Internet gateway is where data stops on its way to or from other networks. Thanks to gateways, we can communicate and send data back and forth with each other.

A gateway, then, is a specific kind of node: It is a computer that sits in between multiple networks, applications, or devices and converts the information and data to the appropriate format or protocol.

Gateways can take several different forms from hardware to software - including routers and computers - and can perform a variety of tasks. These can range from passing traffic to the next 'hop' on its path to filtering traffic, proxies, or protocol translations. Because gateways are, by definition, at the edge of a network, they are often combined with firewalls, which keep out unwanted traffic or 'foreign' computers from a closed network.

At home, the gateway is often the modem (or modem-router combo) provided by your Internet Service Provider (ISP). This gateway allows your computers and devices to connect to the ISP’s network.

At work, the gateway is the computer that routes traffic from a workstation to the outside network that serves up web pages.

A computer-server that is in the role of a gateway may also be a firewall and proxy server. The firewall keeps out unwanted internet traffic and prevents outsiders from accessing private networks.

### **NAT**

NAT stands for network address translation. It’s a way to map multiple private addresses inside a local network to a public IP address before transferring the information onto the internet. 

NAT configurations can reveal just one IP address for an entire network to the outside world as part of this capability, effectively hiding the entire internal network and providing additional security. Network address translation is typically implemented in remote-access environments, as it offers the dual functions of address conservation and enhanced security.

The main use of NAT is to limit the number of public IP addresses an organization or company must use, for both economic and security purposes. 

IP addresses are crucial for internet communication. IPv4 initially provided billions of addresses, but depletion became a concern due to internet expansion. IPv6 was introduced to resolve this issue by offering a more extensive address pool, although its implementation took time. In the interim, Network Address Translation (NAT) was introduced by Cisco and widely adopted as a temporary solution.


### **OSI MODEL**

The Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network. Each layer of the OSI Model handles a specific job and communicates with the layers above and below itself. Although the modern Internet is not based on OSI (but on the simpler TCP/IP model), the OSI Model is still very useful for troubleshooting network problems. 

The 7 layers in the OSI model are:

**7 – Application**

This is where human-computer interaction happens, and this layer is used by end-user software such as web browsers and email clients. As such it provides protocols It provides protocols that allow software to send and receive information and present meaningful data to users such as HTTP, FTP, SMTP, and DNS.

**6 – Presentation**

Layer 6 prepares data for applications, it handles translation, encryption, and compression. It ensures data compatibility between devices with different encoding methods and manages encryption for secure communication. Additionally, it compresses data for more efficient transfer to Layer 5.

**5 – Session**

The session layer creates communication channels, called sessions, between devices. It is responsible for opening sessions, ensuring they remain open and functional while data is being transferred, and closing them when communication ends. The session layer can also set checkpoints during a data transfer—if the session is interrupted, devices can resume data transfer from the last checkpoint.

**4 – Transport**

Layer 4, the transport layer, is responsible for end-to-end communication through segmenting data during transmission and reassembling it on the receiving end. Additionally, it plays a vital role in flow control, ensuring an optimal transmission rate to prevent overwhelming slower receivers. Error control is another responsibility, as it guarantees data completeness and requests retransmissions if necessary for a reliable data transfer process.

**3 – Network**

This layer facilitates data transfer between two different networks and has two main functions. One is breaking up segments into network packets and reassembling the packets on the receiving end. The other is routing packets by discovering the best path across a physical network. The network layer uses network addresses (typically Internet Protocol addresses) to route packets to a destination node.

**2 – Data Link**

The Data Link layer facilitates transfer between two devices on the same network. It breaks packets from layer 3 into smaller pieces, called frames, and sends them to their destination. It is also responsible for flow control and error control in intra-network communication.

**1 – Physical**

This layer includes the physical equipment involved in the data transfer, such as the cables and switches. This is layer converts data into a bit stream, which is a string of 1s and 0s, while taking care of bit rate control.

### **THE TCP/IP MODEL**

TCP/IP is a data link protocol used on the internet to let computers and other devices send and receive data. It is composed of two protocols, TCP or Transmission Control Protocol, and IP or Internet Protocol.

To ensure that each communication reaches its intended destination intact, the TCP/IP model breaks down data into packets and then reassembles the packets into the complete message on the other end. Sending the data in small packets makes it easier to maintain accuracy versus sending all the data at once.

After a single message is split into packets, these packets may travel along different routes before reaching the destination address. Packets may arrive at their destination out of order. IP makes sure the packets arrive at their destination address. TCP puts the packets together in the right order, asks for missing pieces to be resent, and lets the sender know the data has been received. TCP maintains the connection with the sender from before the first packets is sent to after the final one is sent.

The TCP/IP model divides that data into packets according to a four-layer procedure. The data first goes through these layers in one order, and then in reverse order as the data is reassembled on the receiving end.

In the TCP/IP model, the four layers are:

4. Application layer: This corresponds, approximately, to layer 7 in the OSI model.
3. Transport layer: Corresponds to layer 4 in the OSI model.
2. Internet layer: Corresponds to layer 3 in the OSI model.
1. Network access layer: Combines the processes of layers 1 and 2 in the OSI model.

### **TCP/ IP vs OSI**

- Both the TCP/IP and OSI models provide logical ways of networking, as well as the processing of information using a layered system. In both systems, each layer has a specific function. This makes it easier to pinpoint where issues are occurring in the event of a failure.

-	The biggest difference between the two models is that the OSI model segments multiple functions that the TCP/IP model groups into single layers. This is true of both the application and network access layers of the TCP/IP model, which contain multiple layers outlined within the OSI model.


### **DIFFERENCE BETWEEN ASSUME ROLE POLICY AND ROLE POLICY**

***1.	Assume Role Policy:**

-	In AWS IAM, an "assume role policy" is associated with an IAM role. This policy defines which AWS entities (such as AWS users, services, or other accounts) are allowed to assume that role.

-	This policy specifies the conditions under which the role can be assumed. It typically includes a "Principal" element that specifies the entity (e.g., an AWS service or a specific user) that is allowed to assume the role.

-	In Terraform, you can define an IAM role with an `assume_role_policy` block to specify who or what can assume that role.

**2.	Role Policy:**

-	A "role policy" is a set of permissions and access controls that is attached to an IAM role. Once an entity assumes the role, the permissions defined in the role policy determine what actions that entity can perform within AWS services.

-	These policies are similar to standard AWS IAM policies and can be attached to an IAM role using Terraform.

-	In Terraform, you can create an IAM role and attach policies to it using the `aws_iam_role` resource and the `aws_iam_policy_attachment` resource to specify the policies to attach to the role.

To summarize, "assume role policy" is focused on who can assume the role, while "role policy" specifies what actions can be performed after the role is assumed. In Terraform, you can use the AWS provider to define both the IAM role and the policies associated with it, typically by using the `aws_iam_role` resource for the role and `aws_iam_policy_attachment` resource for the policies.
