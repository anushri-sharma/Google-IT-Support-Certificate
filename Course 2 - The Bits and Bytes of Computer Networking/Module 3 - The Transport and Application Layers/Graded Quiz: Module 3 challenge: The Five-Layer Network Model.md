# Graded Quiz: Module 3 challenge: The Five-Layer Network Model

<img width="792" height="508" alt="image" src="https://github.com/user-attachments/assets/fcb3cbac-11ab-4441-b50d-6eba2373cbfb" />

<img width="741" height="354" alt="image" src="https://github.com/user-attachments/assets/f40084d5-5ee4-4040-ac28-d5780d22f51d" />

```
Correct answer: Network A

Why:
Computer 2 has IP: 10.1.1.205
Network A range: 10.1.1.0/24

A /24 subnet means:

Network range: 10.1.1.0 – 10.1.1.255

👉 Since 10.1.1.205 falls within this range, it belongs to Network A
```

<img width="750" height="360" alt="image" src="https://github.com/user-attachments/assets/b81c30c2-a345-42db-aa87-65fc9f23a796" />

```
Since Computer 2 is on a different network, Computer 1 sends the packet to its default gateway
To do that, it needs the MAC address of the gateway
It checks the ARP table to find the MAC address that corresponds to the gateway’s IP
Why others are incorrect:

❌ Port number → used in transport layer (TCP/UDP)
❌ TTL value → related to packet lifetime
❌ Destination MAC address → too vague; specifically it’s the gateway’s MAC address
```

<img width="834" height="610" alt="image" src="https://github.com/user-attachments/assets/fb65ea77-5b94-434a-a696-6b833b9e7980" />

```
Router Z and Computer 2 are on the same network (Network C)
When sending within the same network, the Ethernet frame’s destination MAC must be the final device’s MAC address

Why others are incorrect:

❌ Computer 1’s MAC address → that’s the original sender, not the destination
❌ Router Y’s MAC address → not involved at this stage
❌ No MAC address is needed → Ethernet communication always requires a MAC address

Bottom line:

👉 On the final hop, destination MAC = receiver’s MAC (Computer 2)
```

<img width="739" height="355" alt="image" src="https://github.com/user-attachments/assets/b886e29d-cdc2-43a6-ab17-a04800494e6a" />


```
✅ Computer 2’s MAC address
Since it's on the same network, it sends directly to Computer 2.
```

<img width="844" height="381" alt="image" src="https://github.com/user-attachments/assets/081e4911-a697-4bd4-937a-729f58425171" />

```
When a router (like Router Z) receives an Ethernet frame, the first thing it does is:

Verify the integrity of the frame
It does this by checking the Frame Check Sequence (FCS) (checksum)

Only after confirming the frame is valid does it:

- Remove the Ethernet header
- Look at the IP datagram
- Decrement TTL
- Forward the packet

Why the other options are wrong:

❌ Increases the TTL → TTL is decreased, not increased
❌ Changes destination IP to its own → routers don’t change destination IP
❌ Sends ARP broadcast → happens later if needed, not first
```

<img width="810" height="345" alt="image" src="https://github.com/user-attachments/assets/18282e76-fc35-4902-8de1-5c2ad1d2afba" />

```
TTL (Time To Live) decreases by 1 at each router (hop).

Path:

Computer 1 → Router Y → Router Z → Computer 2

That’s 2 routers, so:

Start TTL = 64
After Router Y → 63
After Router Z → 62
```

<img width="885" height="514" alt="image" src="https://github.com/user-attachments/assets/0e5d5db8-89a9-4a54-8835-5e2a5cbbaec6" />
<img width="823" height="406" alt="image" src="https://github.com/user-attachments/assets/34c77da4-1dcd-4b38-a74a-11634ef58504" />

```
Source Port = 5000 → chosen by Computer 1 (client)
Destination Port = 80 → web server on Computer 2
Sequence Number = 1 → initial sequence number (typical starting point)
Acknowledgment Number = 2 → corresponds to handshake progression
Key idea:
Client → uses a temporary (ephemeral) port
Server → uses a well-known port (80 for HTTP)
Bottom line:

Always remember:
👉 Client port = random (5000 here)
👉 Server port = fixed (80 for web)
```

<img width="865" height="468" alt="image" src="https://github.com/user-attachments/assets/c9ce389a-9807-4862-bb21-3430fd72eadb" />
<img width="773" height="398" alt="image" src="https://github.com/user-attachments/assets/31861b90-bc78-4f47-9409-5da2bc78665a" />

```
Version: 4 → This is an IPv4 address (not IPv6)
Header Length: 20 bytes → Minimum IPv4 header size
Source IP → Must be the sender (192.168.1.121)
Destination IP → Must be the receiver (172.16.1.57)
Why others are incorrect:

❌ Version 5 → doesn’t exist
❌ Header length 32 → not the minimum
❌ Wrong IPs → must match sender/receiver
❌ Version 6 → IPv6 format (not applicable here)

Bottom line:

Always match:
👉 Correct IP version + minimum header + actual source/destination IPs

```

<img width="686" height="361" alt="image" src="https://github.com/user-attachments/assets/272e84ad-d28e-410f-a1f9-95c9d5eff5e1" />

```
The Physical layer is responsible for:

- Transmitting raw bits (1s and 0s)
- Using signals like electrical voltage, light, or radio waves
- Performing modulation to send data over the medium

Why others are incorrect:

❌ Transport → handles ports and reliability (TCP/UDP)
❌ Network → handles IP addressing and routing
❌ Application → user-facing services (browser, email, etc.)
```
