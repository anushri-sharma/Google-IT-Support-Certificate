
# Graded Quiz: Module 4 challenge: Networking Services


<img width="681" height="339" alt="image" src="https://github.com/user-attachments/assets/5942d9e1-d62e-4275-b1f6-d3130e0e7399" />

```
At the lowest level, computers operate using electrical signals:

0 → Off
1 → On

Everything a computer processes (text, images, IP addresses, etc.) is ultimately converted into binary (0s and 1s).
```

<img width="712" height="317" alt="image" src="https://github.com/user-attachments/assets/4c25d2d7-e785-4dec-8711-22263f6f50a5" />

```
💡 Explanation:

There are 13 logical root name servers in the Domain Name System (DNS), labeled:

A.root-servers.net to M.root-servers.net

These are operated by different organizations and distributed worldwide using anycast for reliability and speed.
```

<img width="711" height="335" alt="image" src="https://github.com/user-attachments/assets/d272276d-671f-40fb-ad4c-aa3a40a2cbc5" />

```
💡 Explanation:

DNS (Domain Name System) uses:

Port 53 (UDP) for most name resolution queries (fast, lightweight)
Port 53 (TCP) for larger responses (like zone transfers)

❌ Why others are incorrect:
80 ✖️ → HTTP
22 ✖️ → SSH
25 ✖️ → SMTP (email)
```

<img width="751" height="389" alt="image" src="https://github.com/user-attachments/assets/e8650418-3577-4c50-85fa-ebe556e6dc68" />

```

💡 Explanation:

DNS round robin works by:

Returning multiple IP addresses for the same domain
Rotating the order of those IPs in responses

This helps distribute client requests across multiple servers, effectively doing basic load balancing.

❌ Why others are incorrect:
Redirect traffic from one domain to another ✖️ → That’s URL redirection
Resolve an IP to a domain name ✖️ → That’s reverse DNS
Route traffic based on location/congestion ✖️ → That’s advanced load balancing (not simple round robin)
```

<img width="663" height="318" alt="image" src="https://github.com/user-attachments/assets/c6316c7c-a080-4583-981d-75cbcfce910b" />

```
💡 Explanation:

ICANN is the non-profit organization responsible for:

- Managing and coordinating Top-Level Domains (TLDs) (like .com, .org)
- Overseeing domain name system policies
- Ensuring global uniqueness of domain names

❌ Why others are incorrect:
DHCP ✖️ → Assigns IP addresses
FQDN ✖️ → A full domain name (not an organization)
CNAME ✖️ → A DNS record type
```

<img width="684" height="400" alt="image" src="https://github.com/user-attachments/assets/73d5cf08-1c89-46b2-8e25-0f11dac5a546" />

```
💡 Explanation:

In a DHCPOFFER message:

The DHCP server includes the client’s MAC address (chaddr field)
The client checks this to confirm: “This offer is meant for me”

Since multiple clients may be requesting IPs at the same time, the MAC address uniquely
identifies the intended recipient.

❌ Why others are incorrect:
Client IP address ✖️ → Client doesn’t have one yet
Destination port ✖️ → Same for all DHCP clients
Offered IP address ✖️ → Not used to identify the client
```

<img width="816" height="473" alt="image" src="https://github.com/user-attachments/assets/fc426d1e-30c9-4960-95c1-37ef9e6c5dea" />

```

Explanation
✅ Port Preservation: NAT (specifically Port Address Translation or PAT) allows
multiple devices to use a single public IP address by assigning unique source port
numbers to each session, effectively preserving the limited number of available public IP addresses.

✅ Routable addresses: NAT translates private, non-routable IP addresses
(from a local network) into public, globally routable IP addresses.
This allows devices on a private network to communicate with external
servers on the internet that do not recognize private address ranges.

✅ Address exhaustion: This is the primary problem NAT was designed to solve.
By allowing an entire network of devices to share one or a few public IPv4 addresses,
it significantly slows down the depletion of the limited 32-bit IPv4 address space.

❌ Assigning IPs to devices on the same network: This is incorrect. The assignment
of IP addresses within a local network is typically the responsibility of the
Dynamic Host Configuration Protocol (DHCP), not NAT.
```

<img width="748" height="377" alt="image" src="https://github.com/user-attachments/assets/e5c4192f-1391-4e7b-b220-6de5af94a35f" />

```
💡 Explanation:

With NAT (specifically PAT):

When a client’s source port is available, the router keeps the same port number
This is called port preservation

If the port is already in use, then the router changes it (translation).

❌ Why others are incorrect:
Forwarding ✖️ → Used for directing traffic to internal hosts
Translation ✖️ → General NAT concept, not specific technique
Masquerading ✖️ → A type of NAT, not about keeping the same port
```

<img width="763" height="365" alt="image" src="https://github.com/user-attachments/assets/41026af5-135c-45de-a26f-0fe38d55d6cc" />

```

💡 Explanation:

Most VPNs encapsulate (wrap) an entire packet inside another packet:

They use the payload of the transport layer (TCP/UDP)
Inside that payload is an encrypted packet (new IP + data)

This process is called tunneling.

```

<img width="699" height="374" alt="image" src="https://github.com/user-attachments/assets/52d83d9c-3263-4947-b638-29ee77b925ba" />

```
💡 Explanation:

A web proxy:

Inspects outgoing web requests (like URLs)
Decides whether to allow or block access based on policies
Commonly used in schools and organizations to restrict websites
❌ Why others are incorrect:
Gateway proxy ✖️ → General term, not specific to web filtering
Reverse proxy ✖️ → Protects servers, not clients
Authentication proxy ✖️ → Focuses on verifying user identity
```
