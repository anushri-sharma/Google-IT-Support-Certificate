
# [Practice Quiz: Network Address Translation]


<img width="739" height="364" alt="image" src="https://github.com/user-attachments/assets/1cde2872-8aa4-4fe3-a71a-3c4f77fa7daa" />

```
Port forwarding is a technique where:

- Incoming traffic on a specific port number is redirected
- Sent to a specific device (node) inside a network

📌 Example:
Port 80 → forwarded to a web server
Port 22 → forwarded to an SSH server

❌ Why others are incorrect:

- Ephemeral ports → Temporary ports used by clients
- IP translation (NAT) → Translates IP addresses, not specific ports to nodes
- IP masquerading → A type of NAT, not specific port routing

```

<img width="725" height="359" alt="image" src="https://github.com/user-attachments/assets/d30cc8b9-040b-43f5-9e5c-e8bd3ce8943f" />


```
IP exhaustion happens because IPv4 has a limited number of addresses.

🚀 Solution:
- IPv6 (Internet Protocol version 6) provides a massive address space
- It uses 128-bit addresses (compared to 32-bit in IPv4)
- This creates virtually unlimited public IP addresses

❌ Why others are incorrect:

- IP masquerading → Reuses private IPs using NAT (doesn't create new public IPs)
- Port preservation → Not related to solving IP exhaustion
- RFC1918 → Defines private IP ranges (doesn’t increase public IPs)

```

<img width="729" height="315" alt="image" src="https://github.com/user-attachments/assets/afeffece-830a-4f1f-96b9-f1472f754ad0" />

```
IPv4 uses 32-bit addresses, so the total number of possible addresses is:

2^32 ≈ 4.29×10^9

That’s about 4.2 billion unique IP addresses.
```

<img width="755" height="368" alt="image" src="https://github.com/user-attachments/assets/23b6f205-5903-4671-b423-bb4aed5cda31" />

```
NAT (Network Address Translation) allows a gateway/router to:

Modify (rewrite) the source IP address of outgoing packets
Replace a private IP with a public IP

This is how multiple devices in a private network share one public IP.

❌ Why others are incorrect:
IPv4 / IPv6 → Protocols, they don’t rewrite IPs
IANA → Organization that manages IP allocations
```

<img width="755" height="368" alt="image" src="https://github.com/user-attachments/assets/593ed490-e1e1-4afa-a70a-f88a11f5e792" />

```
ARIN serves:

- United States 🇺🇸
- Canada 🇨🇦
- Parts of the Caribbean

❌ Other options:
- APNIC → Asia-Pacific region
- LACNIC → Latin America
- RIPE NCC → Europe, Middle East, Central Asia
```
