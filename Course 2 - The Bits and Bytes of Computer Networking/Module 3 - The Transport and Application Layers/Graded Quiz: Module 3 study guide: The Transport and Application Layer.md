# Graded Quiz: Module 3 study guide: The Transport and Application Layer


## Question 1 The concept of taking traffic that’s all aimed at the same node and delivering it to the proper receiving service is known as _________.

- demultiplexing
- multiplexing
- encapsulation
- routing

Answer: A. demultiplexing

```

Multiplexing is the process of combining multiple data streams into a single signal
for transmission over a shared medium. Encapsulation involves adding control information
(headers and trailers) to data as it moves through network layers. Routing, typically at
the network layer, determines the best path for data packets to travel across networks to
a destination host. However, the specific process of taking this combined traffic, once it
arrives at the intended node, and separating it to deliver it to the correct receiving application
or service (often identified by port numbers) is called demultiplexing.
```

## Question 2 Which field in the TCP header provides the information for the receiving network device to understand where the actual data payload begins?

- Checksum
- Acknowledgement number
- Data offset
- Sequence number

Answer: D. Data offset

```
The Checksum field is used for error detection, ensuring the integrity of the TCP segment.
The Acknowledgment number confirms the receipt of data from the other end of the connection,
while the Sequence number indicates the order of bytes in the stream. None of these fields
directly specify the start of the data payload. Instead, the TCP header can be of variable
length due to the optional "options" field. To inform the receiving device precisely where
the fixed-size header ends and the actual application data begins, the TCP header includes a
specific field. This field is the Data offset.

```

## Question 3 Which field in a Transmission Control Protocol (TCP) header provides the next expected segment?

- Acknowledgement number
- Sequence number
- Data offset
- Checksum

Answer: A. Acknowledgement number

```
The Sequence number identifies the position of the first byte of data in the current segment
being sent, while the Data offset specifies the length of the TCP header, indicating where the
actual data payload begins. The Checksum field is used for error detection to ensure data integrity.
However, to inform the sending host which byte of data it should transmit next to continue the flow
of communication, TCP utilizes a specific field that indicates the sequence number of the next byte
the receiver expects to get. This field is the Acknowledgement number.

```

## Question 4 The sequence of SYN, SYN/ACK, and ACK packets is known as the _________.

- four-way handshake
- two-way handshake
- high five
- three-way handshake

Answer: D. three-way handshake

```
The initial exchange of packets to establish a TCP connection involves the client
sending a SYN (synchronize) packet, the server responding with a SYN/ACK
(synchronize-acknowledgment) packet, and finally the client sending an ACK (acknowledgment)
packet. This sequence ensures that both sides agree on initial sequence numbers and are
ready to send and receive data reliably. While a "four-way handshake" exists, it refers
to the process of terminating a TCP connection. Therefore, the sequence of SYN, SYN/ACK,
and ACK packets is known as the three-way handshake.

```

## Question 5 A Transmission Control Protocol (TCP) connection is in working order and both sides can send each other data. What is the TCP socket state?

- ESTABLISHED
- LISTEN
- SYN_SENT
- SYN_RECEIVED

Answer: A. ESTABLISHED

```
The LISTEN state indicates that a server socket is waiting for incoming connection requests.
SYN_SENT means a client has sent a SYN packet and is awaiting a SYN/ACK. SYN_RECEIVED signifies
that a server has received a SYN and sent a SYN/ACK, now waiting for the client's final ACK.
When a TCP connection has successfully completed the three-way handshake and is fully established,
allowing both sides to actively exchange data, the socket is in the ESTABLISHED state.

```

## Question 6 If the checksum doesn't compute for a packet sent at the Internet Protocol (IP) level, what will happen to the data?

- The data will be sent back to the sending node with an error.
- The data will be discarded
- The data will be resent
- It will be sent, but may be out of order

Answer: B. The data will be discarded

```
The Internet Protocol (IP) is designed as a best-effort, connectionless protocol,
meaning it doesn't guarantee delivery or provide error recovery mechanisms like retransmission.
Its primary role is to get packets from a source to a destination. If the IP header's checksum
fails to compute correctly, it indicates that the header itself has been corrupted during transit.
Because the IP layer cannot trust the corrupted header information (which contains critical routing
details like the destination address), it does not send the data back for correction, nor does it
attempt to retransmit it. Instead, to prevent misrouting or further network issues from corrupting
data, the data will be discarded.

```

## Question 7 A communication sent through Transmission Control Protocol (TCP) arrives out of order. What allows the data to be put back together in the correct order?

- Acknowledgement number
- Preamble
- Checksum
- Sequence numbers

Answer: D. Sequence numbers

```
The Acknowledgement number is used by the receiver to inform the sender of the next
byte it expects, ensuring reliable flow but not directly reordering. The Preamble is
a synchronization pattern found at the beginning of an Ethernet frame, unrelated to
TCP segment ordering. The Checksum is used for error detection to verify the integrity
of the segment. However, to reconstruct data that might arrive out of sequence, each TCP
segment is assigned a unique identifier indicating the order of the bytes it contains.
This crucial information allows the receiving TCP stack to correctly reassemble the data
stream, even if segments arrive non-sequentially. This is achieved through sequence numbers.
```

## Question 8 In the OSI network model, the ________ is responsible for facilitating the communication between actual applications and the transport layer.

- presentation layer
- physical layer
- application layer
- session layer

Answer: D. session layer

```
The physical layer is concerned with the transmission of raw bits, while the presentation
layer focuses on data formatting, encryption, and compression to ensure data is understandable.
The application layer provides direct network services to end-user applications. However, the layer
specifically tasked with establishing, managing, and terminating the communication dialogue or "session"
between two applications, thereby orchestrating their interaction and ensuring proper synchronization
before handing off to or receiving from the transport layer, is the session layer.

```

## Question 9 Which Transmission Control Protocol (TCP) flag is used to make sure the receiving end knows to examine the sequence number field?

- FIN
- SYN
- PSH
- RST

Answer: B. SYN

```
The FIN flag is used to gracefully close a connection, while PSH requests that data be
immediately delivered to the application. The RST flag is used to abruptly terminate a
connection, often due to an error. However, during the initial phase of connection establishment,
a specific flag is sent to synchronize sequence numbers between the sender and receiver, indicating
that the receiving end should examine the sequence number field. This flag is the SYN flag.

```

## Question 10 You are sending a very small amount of information that you need the listening program to respond to immediately. Which Transmission Control Protocol (TCP) flag will be used?

- ACK
- URG
- PSH
- RST

Answer: C. PSH

```
The ACK flag is used to acknowledge received data, while the RST flag is used to
immediately terminate a connection due to an error. The URG flag indicates that
urgent data is present and should be processed quickly, potentially out of normal
sequence. However, when sending a small amount of information that requires the receiving
application to process and respond without delay, bypassing any buffering delays at the TCP
layer, a specific flag is set to instruct the receiver's TCP stack to deliver the data to the
application immediately. This flag is the PSH flag.

```

## Question 11 Application layer data lives in the _____ section of the transport layer protocol.

- payload
- header
- footer
- flags

Answer: A. payload

```
The header section of a transport layer protocol contains control information necessary
for the protocol's operation, such as source and destination ports, sequence numbers, and
flags, but not the application data itself. A footer, or trailer, is sometimes found in
lower-layer protocols for error checking, but it's not where application data resides in the
transport layer. Flags are specific bits within the header that convey control information.
The actual data originating from the application layer that is being transported by the TCP
or UDP segment is contained within the payload section of the transport layer protocol.

```

## Question 12 What layer of the TCP/IP Five-Layer Network Model allows applications to communicate in a way they understand?

- application
- data-link
- transport
- network

Answer: A. application

```
The data-link layer is responsible for local network communication and framing,
while the network layer handles logical addressing and routing across different networks.
The transport layer provides end-to-end communication between processes on hosts, focusing
on reliability and flow control, but it doesn't interpret the data for applications. The
layer specifically designed to provide services that applications can directly use, enabling
them to communicate using protocols and data formats they understand, is the application layer.
```

## Question 13 Ports that are generally used to establish outbound connections are known as ______ ports.

- registered
- reserved
- ephemeral
- system

Answer: C. ephemeral ports

```
Registered ports (1024-49151) and system/well-known ports (0-1023) are typically used
by specific services for inbound connections, or for outbound connections from specific
client applications. Reserved ports are simply those set aside for future use. However,
when a client program initiates an outbound connection, the operating system dynamically
assigns a temporary port number from a range of high-numbered ports, ensuring unique
identification for that particular connection for its duration. These temporary ports
are known as ephemeral ports.
```

## Question 14 In what order will the Transmission Control Protocol (TCP) generally send all segments?

- Random
- Largest to smallest
- Sequential
- Prioritized

Answer: C. Sequential

```
TCP is a reliable, connection-oriented protocol designed to ensure that data arrives at
its destination completely and in the correct order. Sending segments randomly or from
largest to smallest would lead to significant reordering issues and make reliable reconstruction
of the data nearly impossible. While some applications might prioritize certain data, TCP's
fundamental mechanism for ensuring ordered delivery, which is critical for data integrity,
involves numbering segments and sending them one after another based on those numbers. Therefore,
TCP will generally send all segments in sequential order.
```


## Question 15 A communication between two devices is over the maximum limit of an ethernet frame size. The Transmission Control Protocol (TCP) splits up the data into segments. Which field in the header helps keep track of the many segments?

- Sequence number
- Acknowledgement number
- Checksum
- Urgent pointer

Answer: A. Sequence number

```
The Acknowledgement number is used by the receiver to inform the sender of the next
expected byte, aiding in reliable data flow, but it doesn't primarily track the order
of segments being sent. The Checksum is for error detection, ensuring data integrity,
not segment ordering. The Urgent pointer indicates urgent data within a segment, which is
unrelated to maintaining the order of multiple segments. When a large amount of data needs
to be broken down into smaller pieces to fit within network limitations, TCP assigns a unique
identifier to the beginning of the data within each piece. This crucial field allows the receiving
device to correctly reassemble the segments into their original order, even if they arrive out of
sequence. This field is the Sequence number.

Did``` you completed this study guide?

Yes
