[Basic of Networking](https://www.youtube.com/watch?v=_W7KTBnZqEk&t=8s)

<img width="1270" height="347" alt="image" src="https://github.com/user-attachments/assets/83861075-5341-4a82-94a5-97ac3531213e" />


<img width="1280" height="376" alt="image" src="https://github.com/user-attachments/assets/64d6a4f9-6a9d-4e30-9337-ff50b3deb9d1" />


<img width="1280" height="333" alt="image" src="https://github.com/user-attachments/assets/b64fcb87-123c-4c73-bb36-c9914d49e35d" />


<img width="1280" height="330" alt="image" src="https://github.com/user-attachments/assets/6cf5adc1-fdd7-4595-958c-12da852c4178" />

🔌 Internet as interconnected networks  
  - **Internet = global interconnection of computers/networks**, like a giant spider web linking home, school, workplace, and larger networks into billions of devices.  
  - **Physical components** include **satellites, cellular networks, and buried physical cables** that form the underlying infrastructure.

🌐 World Wide Web vs Internet  
  - **Internet = the physical network infrastructure**; **World Wide Web = the information accessible over that infrastructure**.  
  - Web access typically via browsers (**Firefox, Chrome, Edge**), but **email, chat, and file-sharing** are other Internet services/protocols.

🖥️ Servers, Clients, and ISPs  
  - **Servers**: machines that host and serve content (examples: **Google, Wikipedia, Reddit, BBC**).  
  - **Clients**: user devices (phones, laptops, game consoles) that request content from servers.  
  - **ISPs (Internet Service Providers)** (examples: **CenturyLink, Level 3, Comcast, Telefónica**) operate networks, deploy cabling, and interconnect with other ISPs and networks so clients can reach servers.

🧾 Addressing: IP addresses and MAC addresses  
  - **IP address**: network-level identifier used for routing across networks (example **100.1.4.3**, **172.217.6.46**); analogous to a house address.  
  - **MAC address**: hardware-level identifier for a network interface (example **82:4f:23:59:47:4**); analogous to the recipient name; usually assigned to the device and often persistent.  
  - Devices typically require **both an IP (for routing between networks)** and a **MAC (for local delivery on a LAN)** to communicate.  
  - Layering nuance: **MAC = link layer (Layer 2)**, **IP = network layer (Layer 3)**; local mechanisms (e.g., ARP) map IP → MAC so packets can be delivered on the local segment.

✉️ Routing explained via postal analogy  
  - Sender writes **recipient name + address**; mail passes through multiple hubs where workers forward it based on where the next transport is headed.  
  - Each intermediate hop forwards toward a nearer destination (truck to Texas, truck to San Francisco, plane to Tokyo), and final local delivery occurs when the packet reaches the destination's local network.  
  - Implication: **Internet routing is hop-by-hop**, with routers forwarding packets toward the destination until the final network can deliver them.

📦 Packets and data transport  
  - All data is divided into **packets** (small units of binary data) regardless of type (images, email, music, text).  
  - Packets can take different paths and are **reassembled** into the original data at the destination.  
  - Analogy: each packet is like an individual letter; many letters together form the full message.

🔀 Example flow: Natalie requests Google  
  - Natalie’s device (**IP 113.8.81.2**) wants to reach **google.com (IP 172.217.6.46)** to fetch cat pictures.  
  - Her device sends a packet toward that IP; intermediate routers forward the packet hop-by-hop, each moving it closer until it reaches a network that can deliver to Google’s servers.  
 

<img width="1272" height="490" alt="image" src="https://github.com/user-attachments/assets/214ec861-a50d-41c3-9e62-4a84f8e555a4" />

 - Google responds with packets that traverse back and are reassembled on Natalie’s device, delivering the requested content.


<img width="1275" height="454" alt="image" src="https://github.com/user-attachments/assets/85e2c24e-ac24-4fbf-948f-8beb9b2c37dc" />

🎓 Networking as an IT discipline  
  - **Networking** covers designing, building, and managing networks; it is a substantial IT domain with dedicated jobs, degree programs, and extensive literature.  
  - Understanding networking fundamentals is essential for IT professionals.
