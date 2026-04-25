
# Graded Quiz: Module 6 challenge: Troubleshooting and the Future of Networking


<img width="649" height="301" alt="image" src="https://github.com/user-attachments/assets/f5ee2c52-b2e9-4b08-b49b-96f713ef6220" />

```
A Cyclic Redundancy Check (CRC) is used to detect errors in data transmission.
It adds a checksum to data, and the receiver recalculates it to verify integrity.

Why others are incorrect:
Misconfiguration error → not related to CRC
Time To Live (TTL) expiration → relates to packet lifetime, not data integrity
Error recovery → CRC detects errors but does not fix them

```

<img width="749" height="431" alt="image" src="https://github.com/user-attachments/assets/07efc5e2-036e-45ea-aff3-78ed95ed267a" />

```
Why these are correct:

These are standard ICMP message types used for network diagnostics:

- Destination unreachable → sent when a packet cannot reach its destination
- Time exceeded → sent when the TTL value reaches zero (used in traceroute)

❌ Why the others are incorrect:

- HTTP 404 Not Found → this is an HTTP status code, not ICMP
- ARP request failed → ARP is a different protocol, not ICMP
```

<img width="723" height="333" alt="image" src="https://github.com/user-attachments/assets/badc56d0-39b5-4e26-9892-3b9eb0e97081" />

```
Why:
- On Windows, the equivalent of traceroute (Linux/macOS) is tracert.
- It performs the same function—tracking the path packets take across a network.

Why others are incorrect:

- Tracepath → Linux tool, not Windows
- Ping → checks connectivity, not route path
- ipconfig → displays network configuration
```

<img width="729" height="339" alt="image" src="https://github.com/user-attachments/assets/64bc2cc7-10b3-4258-9ab5-69ceae8c478a" />

```
Why:

When you run Test-NetConnection with only a hostname, it performs a basic connectivity
test—similar to ping—by sending an ICMP Echo Request.

Why others are incorrect:

- Network address translation → unrelated to this command’s default behavior
- Name server lookup → DNS resolution may happen, but it’s not the main test action
- Private tunnel → not part of this command

✔️ Final answer: ICMP Echo request
```


<img width="693" height="304" alt="image" src="https://github.com/user-attachments/assets/959cd3ef-5e65-47d2-8d04-caa1d0a53c5b" />

```
Why:

- Nslookup is one of the most commonly used tools to query DNS and perform name resolution (domain → IP).

Why others are incorrect:

- DNS → it’s the system/protocol, not a tool
- Netcat → used for networking/debugging, not name resolution
- Tracert → traces network path, not DNS queries

```

<img width="717" height="330" alt="image" src="https://github.com/user-attachments/assets/abe974aa-f2a7-4866-9e0b-6209cfc8bca8" />

```
Why:
Google provides two well-known public DNS servers:

-  8.8.8.8
-  8.8.4.4


Why others are incorrect:
 - 0.0.0.0 → represents an unspecified address
 - 255.255.255.255 → broadcast address
 - 1.2.1.1 → not a public DNS server

✔️ Final answer: 8.8.4.4

```

<img width="699" height="344" alt="image" src="https://github.com/user-attachments/assets/b4ba7958-ba72-4bc7-ad94-6ef338eabc5e" />

```
In virtualization:

- The host is the physical machine
- The guests are the virtual machines (VMs) running on that host

Why others are incorrect:
- Servers → too general
- Clouds → not a VM term
- Clients → refers to end-user devices

```

<img width="682" height="304" alt="image" src="https://github.com/user-attachments/assets/72992ecb-ecc5-4da7-b4fc-f775cf3d0439" />

```
Why:

- This is the IPv6 loopback address, commonly written in shorthand as ::1
- It serves the same purpose as 127.0.0.1 in IPv4 (refers to the local machine)

Why others are incorrect:

- 127.0.0.1 → IPv4 loopback, not IPv6
- 0000:...:0000 → unspecified address (::), not loopback
- 1000:...:0000 → not a valid loopback address
```

<img width="713" height="321" alt="image" src="https://github.com/user-attachments/assets/aaba3fce-fcfd-4b81-87f0-b15e7af87cf8" />

```
Why this is correct:

To compress an IPv6 address:

1. Remove leading zeros in each block
    - 00a9 → a9, 00fd → fd, 0358 → 358, 0000 → 0
2. Replace one consecutive block of zeros (0000) with :: (only once)

So:
7d2b:00a9:a0c4:0000:a772:00fd:a523:0358
→ 7d2b:a9:a0c4::a772:fd:a523:358

```

<img width="736" height="322" alt="image" src="https://github.com/user-attachments/assets/509fa813-ec7d-4d86-a3cf-5782427b732d" />

```
In IPv6, the Payload Length field is 16 bits long and specifies the size
of the data following the IPv6 header.

❌ Why others are incorrect:

- 20-bit → not used in IPv6 header
- 32-bit → too large for this field
- 8-bit → too small
```
