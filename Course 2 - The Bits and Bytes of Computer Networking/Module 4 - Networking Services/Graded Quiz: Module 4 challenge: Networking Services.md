
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

<img width="861" height="369" alt="image" src="https://github.com/user-attachments/assets/dfc52726-54dc-4964-8336-335491df03d8" />

```
💡 Explanation:

When a website is moved to a new web host:

- The server changes, so the IP address associated with the domain changes
- The domain name (like example.com) usually stays the same
- DNS records are updated to point to the new IP

❌ Why others are incorrect:

- Root name server ✖️ → Unrelated to individual websites
- Network service ✖️ → Not necessarily changed
- Domain name ✖️ → Typically remains the same
```

<img width="817" height="377" alt="image" src="https://github.com/user-attachments/assets/8dd13486-6f38-4099-9169-92500b3c75ad" />

```
A CNAME (Canonical Name) record maps one domain name to another
```

<img width="816" height="348" alt="image" src="https://github.com/user-attachments/assets/ce55fe13-5041-4235-987a-bebfc7bb2202" />


```
💡 Explanation:

When NAT hides the original (private) source IP and replaces it with the router’s public IP, it’s called masquerading.

Internal device → private IP
Router → replaces it with public IP
External network only sees the router’s IP
```

<img width="854" height="406" alt="image" src="https://github.com/user-attachments/assets/8e5cb49c-c7b7-4223-8762-054a630ee4b8" />

```
💡 Explanation:

NAT masquerading (one-to-many NAT) hides all internal IPs behind one public IP
But to allow incoming traffic (like hosting a web server), you need a way to direct
requests to the correct internal device
Port forwarding does exactly that:

- Maps a specific port on the public IP
- Forwards it to a specific internal IP + port

❌ Why others are incorrect:

Preservation ✖️ → Refers to keeping the same port number
One-to-many ✖️ → Describes NAT type, but doesn’t handle incoming traffic routing
Rewriting ✖️ → General concept, not a specific technique
```

<img width="750" height="376" alt="image" src="https://github.com/user-attachments/assets/40d74817-88d7-47bd-9dee-2eb8c92e3984" />


```
💡 Explanation:

A reverse proxy:

- Appears as a single server to clients
- Forwards requests to multiple backend servers
- Helps with load balancing, security, and performance

❌ Why others are incorrect:

- multiplexer ✖️ → Not used in this context
- VPN ✖️ → Secure connection, not request distribution
- port preservation ✖️ → NAT concept
```
