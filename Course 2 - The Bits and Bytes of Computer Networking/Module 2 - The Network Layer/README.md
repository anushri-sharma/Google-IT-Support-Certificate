## The Network Layer

In the second week of this course, we'll explore the network layer in more depth. We'll learn about the IP addressing scheme and how subnetting works. We'll explore how encapsulation works and how protocols such as ARP allow different layers of the network to communicate. We'll also cover the basics of routing, routing protocols, and how the Internet works. By the end of this module, you'll be able to describe the IP addressing scheme, understand how subnetting works, perform binary math to describe subnets, and understand how the Internet works.

### Key Concepts

* Describe the IP addressing scheme.
* Describe how subnetting works.
* Describe subnets by performing basic math in binary.
* Demonstrate how encapsulation works.
* Describe how ARP protocols allow different layers of the network to communicate.
* Describe how the Internet works.
* Understand the basics of routing and routing protocols. 

------


## Module Highlights

### The Network Layer

* On a local area network or LAN, nodes can communicate with each other through their physical MAC addresses. But MAC addressing isn't a scheme that scales well, every single network interface on the planet has a unique MAC address and they aren't ordered in any systematic way.
* **IP addresses** are a 32 bit long numbers made up of four octets, and each octet is normally described in decimal numbers. 8 bits of data or a single octet can represent all decimal numbers from 0 to 255.
* 12.30.56.78 is a valid IP address, but 123.456.789.100 would not be because it has numbers larger than could be represented by 8 bits. This format is known as **dotted decimal notation**. 
* **IP addresses** are distributed in large sections to various organizations and companies instead of being determined by hardware vendors. This means that IP addresses are more hierarchical and easier to store data about than physical addresses are.
* IP addresses belong to networks, not to the devices attached to those networks.
Many modern networks you can connect a new device and an IP address will be assigned to it automatically through a technology known as **dynamic host configuration protocol**. An IP address assigned this way is known as a **dynamic IP address**. 
* In most cases static IP addresses are reserved for servers and network devices, while dynamic IP addresses are reserved for clients. But there are certainly situations where this might not be true. 
* Under the IP protocol, a packet is usually referred to as an **IP datagram**. Just like any Ethernet frame, an IP datagram is a highly structured series of fields that are strictly defined. 
* **IP datagram**: A highly structured series of fields that are strictly defined.
* The most common version of **IP** is version 4, or **IPv4**.
* **Header Length field**: Almost always 20 bytes in length when dealing with IPv4. 20 bytes is the minimum length of an IP header.
* **Service Type field**: These 8 bits can be used to specify details about quality of servicem or QoS technologies.
* **Total Length field**: Indicates the total length of the IP datagram it's attached to.
* **Identification field**: A 16-bit number that's used to group messages together.
* The maximum size of a single datagram is the largest number you can represent with 16 bits: 65,535.
* If the total amount of data that needs to be sent is larget than what can fit in a single datagram, the IP layer needs to split this data up into many individual packets.
* **Flag field**: Used to indicate if a datagram is allowed to be fragmented, or to indicate that the datagram has already been fragmented.
* **Fragmentation**: The process of taking a single IP datagram and splitting it up into several smaller datagrams.
* **Time to Live (TTL) field**: An 8-bit field that indicates how many router hops a datagram can traverse before it's thrown away.
* **Protocol field**: Another 8-bit field that contains data about what transport layer protocol is being used.
* The most common transport layer protocols are **TCP** and **UDP**.
* **Header checksup field**: A checksum of the contents of the entire IP datagram header.
* **IP options field**: An optional field and is used to set special characteristics for datagram primarily used for testing purposes.
* **Padding field**: A series of zeros used to ensure the header is the correct total size.
* IP addresses can be split into two sections, the **network ID** and the **host ID**. 
* In IP address, the network ID would be the first octet, and the host ID would be the second, third and fourth octets.
* There are three primary types of address classes.
  * **Class A** addresses are those where the first octet is used for the network ID and the last three are used for the host ID.
  * **Class B** addresses are where the first two octets are used for the network ID, and the second two are used for the host ID.
  * **Class C** addresses, as you might have guessed, are those where the first three octets are used for the network ID, and only the final octet is used for the host ID. 
* If the very first bit of an IP address is 0, it belongs to a **Class A** network. 0.0.0.0 - 127.255.255.255.
* If the first bits are 10, it belongs to a **Class B** network. 128.255.255.255 - 191.255.255.255.
* If the first bits are 110, it belongs to a **Class C** network. 192.255.255.255 - 223.255.255.255.
* **ARP**: A protocol used to discover the hardware address of a node with a certain IP address.
* Almost all network connected devices will retain a local ARP table. 
* **APR table**: A list of IP addresses an the MAC addresses associated with them. 
* ARP table entries generally expire after a short amount of time to ensure changes in the network are accounted for.

### Subnetting

* **Subnetting**: The process of taking a large network and splitting it up into many individual and smaller subnetworks or subnets.
* Incorrect subnetting setups are a common problem you might run into as an IT Support Specialist, so it's important to have a strong understanding of how this works.
* **Network IDs** are used to identify networks, and **Host IDs** are used to identify individual hosts. 
* **Subnet masks**: 32-bit numbers that are normally written now as four octets in decimal.
* A single 8-bit number can represent 256 different numbers, or more specifically, the numbers 0-255.
* The network ID is always either 8 bit for class A networks, 16 bit for class B networks, or 24 bit for class C networks.
* **Demarcation point**: To describe where one network or system ends and another one begins.

### Routing

* The way communications happen across all these networks, allowing you to access data from the other side of the planet, is through **routing**.
* Along with managing IP address allocation, the **IANA** is also responsible for **ASN**, or **Autonomous System Number** allocation.
* **Autonomous System Number (ASN)**: Numbers assigned to individual autonomous systems.
* **Transport layer**: Allows traffic to be directed to specific network applications.
* **Application layer**: Allows these applications to communicate in a way they understand.

-----


Address class system: A system which defines how the global IP address space is split up

Address Resolution Protocol (ARP): A protocol used to discover the hardware address of a node
with a certain IP address

ARP table: A list of IP addresses and the MAC addresses associated with them

ASN: Autonomous System Number is a number assigned to an individual autonomous system

Demarcate: To set the boundaries of something

Demarcation point: Where one network or system ends and another one begins

Destination network: The column in a routing table that contains a row for each network that the
router knows about

DHCP: A technology that assigns an IP address automatically to a new device. It is an application layer
protocol that automates the configuration process of hosts on a network

Dotted decimal notation: A format of using dots to separate numbers in a string, such as in an IP
address

Dynamic IP address: An IP address assigned automatically to a new device through a technology
known as Dynamic Host Configuration Protocol

Exterior gateway: Protocols that are used for the exchange of information between independent
autonomous systems

Flag field: It is used to indicate if a datagram is allowed to be fragmented, or to indicate that the
datagram has already been fragmented

Fragmentation: The process of taking a single IP datagram and splitting it up into several smaller
datagrams

Fragmentation offset field: It contains values used by the receiving end to take all the parts of a
fragmented packet and put them back together in the correct order

Header checksum field: A checksum of the contents of the entire IP datagram header

Header length field: A four bit field that declares how long the entire header is. It is almost always 20
bytes in length when dealing with IPv4

IANA: The Internet Assigned Numbers Authority, is a non-profit organization that helps manage things
like IP address allocation

Identification field: It is a 16-bit number that's used to group messages together

Interface: For a router, the port where a router connects to a network. A router gives and receives
data through its interfaces. These are also used as part of the routing table

Interior gateway: Interior gateway protocols are used by routers to share information within a single
autonomous system

IP datagram: A highly structured series of fields that are strictly defined

IP options field: An optional field and is used to set special characteristics for datagrams primarily
used for testing purposes

Network Address Translation (NAT): A mitigation tool that lets organizations use one public IP
address and many private IP addresses within the network

Next hop: The IP address of the next router that should receive data intended for the destination
networking question or this could just state the network is directly connected and that there aren't any
additional hops needed. Defined as part of the routing table

Non-routable address space: They are ranges of IPs set aside for use by anyone that cannot be
routed to

Padding field: A series of zeros used to ensure the header is the correct total size

Protocol field: A protocol field is an 8-bit field that contains data about what transport layer protocol
is being used

Routing protocols: Special protocols the routers use to speak to each other in order to share what
information they might have

Service type field: A eight bit field that can be used to specify details about quality of service or QoS
technologies

Static IP address: An IP address that must be manually configured on a node

Subnet mask: 32-bit numbers that are normally written as four octets of decimal numbers

Subnetting: The process of taking a large network and splitting it up into many individual smaller sub
networks or subnets

Time-To-Live field (TTL): An 8-bit field that indicates how many router hops a datagram can traverse
before it's thrown away

Total hops: The total number of devices data passes through to get from its source to its destination.
Routers try to choose the shortest path, so fewest hops possible. The routing table is used to keep
track of this

Total length field: A 16-bit field that indicates the total length of the IP datagram it's attached to
