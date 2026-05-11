## Introduction to Networking

Welcome to the Networking course of the IT Support Professional Certificate! In the first week of this course, we will cover the basics of computer networking. We will learn about the TCP/IP and OSI networking models and how the network layers work together. We'll also cover the basics of networking devices such as cables, hubs and switches, routers, servers and clients. We'll also explore the physical layer and data link layer of our networking model in more detail. By the end of this module, you will know how all the different layers of the network model fit together to create a network.

### Key Concepts

* Describe how the TCP/IP five layer network model works.
* Identify basic networking devices.
* Label each of the five layers in the TCP/IP network model.
* Describe how the physical layer works.
* Describe how the data link layer works.

-----

## Module Highlights

<br>

### The TCP/IP Five-Layer Network Model

* Five-layer model for networking:
  * Physical layer.
  * Data link layer.
  * Network layer.
  * Transport layer.
  * Application layer.
* **Physical layer**: Represent the physical devices that interconnect computers, is about cabling, connectors and sending signals.
* **Data link layer**: Responsible for defining a common way of interpreting these signals so network devices can communicate. **Ethernet** is an example of a transport layer protocol.
* The **Ethernet** standards also define a protocol responsible for getting data to nodes on the same network or link.
* **Network layer**: Allows different networks to communicate with each other through device known as routers. **IP** is the most common network layer protocol.
* **Internetwork**: A collection of networks connected together through routers, the most famous of these being the **Internet**.
* While the **data link layer** is responsible for getting data across a single link, the **network layer** is responsible for getting data delivered across a collection of networks. 
* **IP** is the heart of the Internet and most smaller networks around the world.
* **Transport layer**: Sorts out which client and server programs are supposed to get that data. **TCP** is an example of a transport layer protocol.
* Other transfer protocols also use **IP** to get around, including a protocol known as **User Datagram Protocol (UDP)**. 
* **TCP** provides mechanisms to ensure that data is reliably delivered while **UDP** does not. 
* **IP** is responsible for getting data from one node to another. 
* You can think of layers like different aspects of a package being delivered. The **physical layer** is the delivery truck and the roads. The **data link layer** is how the delivery trucks get from one intersection to the next over and over. The **network layer** identifies which roads need to be taken to get from address A to address B. The **transport layer** ensures that delivery driver knows how to knock on your door to tell you your package has arrived. And the **application layer** is the contents of the package itself. 

<br>

### The Basics of Networking Devices

* **Cables**: Connect different devices to each other, allowing data to be transmitted over them.
* Most network cables used today can be divided into two categories, **copper** and **fiber**.
* The most common form of copper twisted-pair cables used in networking are **Cat5**, **Cat5e**, and **Cat6** cables.
* **Crosstalk**: When an electrical pulse on one wire is accidentally detected on another wire.
* **Fiber cables**: Contain individual optical fibers, which are tiny tubes made out of glass about the width of a human hair.
* Unlike copper, which uses **electrical voltages**,
fiber cables use **pulses of light** to represent the zeros and one of the data they transmit.
* **Hub**: A physical layer device that allows for connections from many computers at once.
* **Collision domain**: A network segment where only one device can communicate at a time.
* If multiple system try sending data at the same time, the electrical pulse sent across the cable can interfere with each other. This causes these systems to have to wait for a quiet period before they try sending their data again.
* A **switch** is very similar to a **hub** since you can connect many devices to it so they can communicate.  The difference is that while a hub is a layer one or **physical layer** device, a switch is a layer two or **data link** device. This means that a switch can actually inspect the contents of the ethernet protocol data being sent around the network.
* **Hub and switches**: The primary devices used to connect on a single network, usually referred to as a **LAN**, or **local area network**.
* **Router**: A device that knows how to forward data between independent networks.
* Just like a **switch** can inspect Ethernet data to determine where to send things, a **router** can inspect IP data to determine where to send things. 
* **Border Gateway Protocol (BGP)**: Routers share data with each other via this protocol, which lets them learn about the most optimal paths to forward traffic.
* In most network topographies, each node is primarily either a server, or a client. 

<br>

### The Physical Layer

* **Bit**: The smallest representation of data that a computer can understand; it's a one or a zero.
* A standard copper network cable, once connected to devices on both ends, will carry a constant electrical charge. Ones and zeros are sent across those network cables through a process called **modulation**
* **Modulation**: A way of varying the voltage of this carge moving across the cable.
* The most common type of cabling used for connecting computing devices is known as **twisted pair**. It's called a twisted pair cable because it features pairs of copper wires that are twisted together. 
* **Duplex communication**: The concept that information can flow in both directions across the cable.
* **Simplex communication**: This process is unidirectional.
* **Full duplex**: Devices on either side of a networking link can both communicate with each other at the exact same time.

<br>

### The Data Link Layer

* The protocol most widely used to send data across individual links is known as **Ethernet**.
* **Ethernet** and the **data link** layer provide a means for software at higher levels of the stack to send and receive data. 
* If two computers were to send data across the wire at the same time, this would result in literal collisions of the electrical current representing our ones and zeros, leaving the end result unintelligible. 
* Ethernet as a protocol solved this problem by using a technique known as carrier sense multiple access with collision detection.
* **CSMA/CD**: Used to determine when the communications channel are clear, and when a device is free to transmit data.
* **MAC address**: A global unique identifier attached to an individual network interface. It's a 48-bit number normally represented by six groupings of two hexadecimal numbers.
* **Hexadecimal**: A way to represent number using 16 digits.
* **Octet**: In computer networking, any number that can be represented by 8 bits.
* Organizationally Unique Identifier (OUI): The first three octets of a MAC address.
* If the least significant bit in the first octet of a destination address is set to **zero**, it means that ethernet frame is intended for **only the destination address**.
* IF the least significant bit in the first octet of a destination address is set to **one**, it means you're dealing with a **multicast frame**.
* **Data packet**: An all-encompassing term that represents any single set of binary data being sent across a network link.
* Data packets at the Ethernet level are known as **Ethernet frames**.
* **Ethernet frame**: A highly structured collection of information presented in a specific order.
* The first part of an Ethernet frame is known as the **preamble**. A preamble is 8 bytes or 64 bits long and can itself be split into two sections. 
* **Start frame delimiter (SFD)**: Signals to a receiving device that the preamble is over and that the actual frame contents will now follow.
* **Destination MAC address**: The hardware address of the intended recipient.
* **EtherType field**: 16 bits long and used to describe the protocol of the contents of the frame.
* **VLAN header**: Indicates that the frame itself is what's called VLAN frame
* If a VLAN header is present, the EtherType field follows it.
* **Virtual LAN (VLAN)**: A technique that lets you have multiple logical LANs operating on the same physical equipment.
* **Frame Check Sequence**: A 4-byte (or 32-bit) number that represents a checksum value for the entire frame.
* **Checksum value** is calculated by performing what's known as a cyclical redundancy check against the frame.
* **Cyclical Redudancy Check (CRC)**: An important concept for data integrity and is used all over computing, not just network transmissions.

-----


Bit: The smallest representation of data that a computer can understand

Border Gateway Protocol (BGP): A protocol by which routers share data with each other

Broadcast: A type of Ethernet transmission, sent to every single device on a LAN

Broadcast address: A special destination used by an Ethernet broadcast composed by all Fs

Cable categories: Groups of cables that are made with the same material. Most network cables used
today can be split into two categories, copper and ber

Cables: Insulated wires that connect dierent devices to each other allowing data to be transmied
over them

Carrier-Sense Multiple Access with Collision Detection (CSMA/CD): CSMA/CD is used to
determine when the communications channels are clear and when the device is free to transmit data

Client: A device that receives data from a server

Collision domain: A network segment where only one device can communicate at a time

Computer networking: The full scope of how computers communicate with each other

Copper cable categories : These categories have dierent physical characteristics like the number of
twists in the pair of copper wires. These are dened as names like category (or cat) 5, 5e, or 6, and
how quickly data can be sent across them and how resistant they are to outside interference are all
related to the way the twisted pairs inside are arranged

Crosstalk: Crosstalk is when an electrical pulse on one wire is accidentally detected on another wire

Cyclical Redundancy Check (CRC): A mathematical transformation that uses polynomial division to
create a number that represents a larger set of data. It is an important concept for data integrity and is
used all over computing, not just network transmissions

Data packet: An all-encompassing term that represents any single set of binary data being sent
across a network link

Datalink layer: The layer in which the rst protocols are introduced. This layer is responsible for
dening a common way of interpreting signals, so network devices can communicate

Destination MAC address: The hardware address of the intended recipient that immediately follows
the start frame delimiter

Duplex communication: A form of communication where information can ow in both directions
across a cable

Ethernet: The protocol most widely used to send data across individual links

Ethernet frame: A highly structured collection of information presented in a specic order

EtherType eld: It follows the Source MAC Address in a dataframe. It's 16 bits long and used to
describe the protocol of the contents of the frame

Fiber cable: Fiber optic cables contain individual optical bers which are tiny tubes made of glass
about the width of a human hair. Unlike copper, which uses electrical voltages, ber cables use pulses
of light to represent the ones and zeros of the underlying data

Five layer model: A model used to explain how network devices communicate. This model has ve
layers that stack on top of each other: Physical, Data Link, Network, Transport, and Application

Frame check sequence: It is a 4-byte or 32-bit number that represents a checksum value for the
entire frame

Full duplex: The capacity of devices on either side of a networking link to communicate with each
other at the exact same time

Half-duplex: It means that, while communication is possible in each direction, only one device can be
communicating at a time

Hexadecimal: A way to represent numbers using a numerical base of 16

Hub: It is a physical layer device that broadcasts data to every computer connected to it

Internet Protocol (IP): The most common protocol used in the network layer

Internet Service Provider (ISP): A company that provides a consumer an internet connection

Internetwork: A collection of networks connected together through routers - the most famous of
these being the Internet

Line coding: Modulation used for computer networks

Local Area Network (LAN): A single network in which multiple devices are connected

MAC(Media Access Control) address: A globally unique identier aached to an individual network
interface. It's a 48-bit number normally represented by six groupings of two hexadecimal numbers

Modulation: A way of varying the voltage of a constant electrical charge moving across a standard
copper network cable

Multicast frame: If the least signicant bit in the rst octet of a destination address is set to one, it
means you're dealing with a multicast frame. A multicast frame is similarly set to all devices on the
local network signal, and it will be accepted or discarded by each device depending on criteria aside
from their own hardware MAC address

Network layer: It's the layer that allows dierent networks to communicate with each other through
devices known as routers. It is responsible for geing data delivered across a collection of networks

Network port: The physical connector to be able to connect a device to the network. This may be
aached directly to a device on a computer network, or could also be located on a wall or on a patch
panel

Network switch: It is a level 2 or data link device that can connect to many devices so they can
communicate. It can inspect the contents of the Ethernet protocol data being sent around the network,
determine which system the data is intended for and then only send that data to that one system

Node: Any device connected to a network. On most networks, each node will typically act as a server
or a client

Octet: Any number that can be represented by 8 bits

Organizationally Unique Identier (OUI): The rst three octets of a MAC address

OSI model: A model used to dene how network devices communicate. This model has seven layers
that stack on top of each other: Physical, Data Link, Network, Transport, Session, Presentation, and
Application

Patch panel: A device containing many physical network ports

Payload: The actual data being transported, which is everything that isn't a header

Physical layer: It represents the physical devices that interconnect computers

Preamble: The rst part of an Ethernet frame, it is 8 bytes or 64 bits long and can itself be split into
two sections

Protocol: A dened set of standards that computers must follow in order to communicate properly is
called a protocol

Router: A device that knows how to forward data between independent networks

Server: A device that provides data to another device that is requesting that data, also known as a
client

Simplex communication: A form of data communication that only goes in one direction across a
cable

Source MAC address: The hardware address of the device that sent the ethernet frame or data
packet. In the data packet it follows the destination MAC address

Start Frame Delimiter (SFD): The last byte in the preamble, that signals to a receiving device that the
preamble is over and that the actual frame contents will now follow

Transmission Control Protocol (TCP): The data transfer protocol most commonly used in the fourth
layer. This protocol requires an established connection between the client and server

Transport layer: The network layer that sorts out which client and server programs are supposed to
get the data

Twisted pair cable: The most common type of cabling used for connecting computing devices. It
features pairs of copper wires that are twisted together

Unicast transmission: A unicast transmission is always meant for just one receiving address

User Datagram Protocol (UDP): A transfer protocol that does not rely on connections. This protocol
does not support the concept of an acknowledgement. With UDP, you just set a destination port and
send the data packet

Virtual LAN (VLAN): It is a technique that lets you have multiple logical LANs operating on the same
physical equipment

VLAN header: A piece of data that indicates what the frame itself is. In a data packet it is followed by
the EtherType
