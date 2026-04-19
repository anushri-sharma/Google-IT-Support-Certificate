[Networking Hardware](https://www.youtube.com/watch?v=KpnJssiJ8kQ&t=3s)

<img width="1280" height="305" alt="image" src="https://github.com/user-attachments/assets/f38a6dcf-264d-438d-b123-9cf443667055" />


<img width="1280" height="355" alt="image" src="https://github.com/user-attachments/assets/f3287602-b6da-4396-ad06-f3277ed662f1" />


🔌 Ethernet (wired connection)  
  – **Physical cable** that connects a computer to the network via a **network port** on the device (e.g., desktop back panel).  
  – Uses electrical signals over copper wiring to carry data.  
  – Common for stable, low-latency connections.

📶 Wi‑Fi (wireless connection)  
  – **Wireless networking** that connects devices via **radios and antennas**.  
  – Built into most modern devices (mobile phones, smart TVs, laptops).  
  – Trades convenience and mobility for potential variability in speed and signal quality.

🔬 Fiber optic (high‑speed wired connection)  
  – Uses **glass fibers** to transmit data as **light** rather than electrical current.  
  – Sends binary data (“ones and zeros”) using a **beam of light** through the fiber.  
  – **Higher speeds** and longer-distance performance than copper; typically **more expensive**.

🖧 Network devices: why cables don’t connect every computer directly  
  – Computers connect to intermediary **devices that organize and direct traffic** instead of directly to every other computer.  
  – This reduces cabling complexity and enables scalable network management.

🛣️ Routers (directing traffic between networks and to the Internet)  
  – **Connects multiple devices and networks** and uses **network protocols** to determine where to send packets.  
  – Example: sending a file from **Computer A to Computer B** in the same network — the packet goes through the router and is routed to B.  
  – For a destination on a different network (e.g., **Alejandro’s computer**), the router forwards packets **out of the local network to the ISP** and onward across multiple networks.

<img width="1280" height="534" alt="image" src="https://github.com/user-attachments/assets/cb087749-5e37-4732-9725-7b58e1f6c704" />


🔀 Switches vs hubs (internal network traffic behavior)  
  – **Switches**: direct traffic selectively—analogy: **mail room** that delivers mail to the correct recipient inside a building.  
  – **Hubs**: broadcast traffic to all connected devices—analogy: **company memos** sent to everyone regardless of intended recipient.  
  – Switches are used when targeted delivery and efficiency are required; hubs create unnecessary traffic.

📡 Packet path and multiple devices  
  – A packet traveling off‑network typically traverses **many routers, switches, and hubs** en route to its destination.  
  – Each device along the path performs a role in forwarding or delivering the packet according to protocol rules.

🛠️ Troubleshooting and the network stack (investigation order and definition)  
  – **Network stack**: the set of hardware and software components that provide networking infrastructure.  
  – When users report Internet access problems, **investigate upward through the stack**:  
    – **End‑user computer(s)** first (local configuration, NICs, OS).  
    – Then physical infrastructure: **cabling**, **switches**, **routers**.  
  – Systematic escalation through those layers helps isolate points of failure.

<img width="1278" height="431" alt="image" src="https://github.com/user-attachments/assets/aaa1370d-ec76-4221-b98a-a6c236caa52b" />
