
[History of Internet](https://www.youtube.com/watch?v=4kkzoSRPaoo&t=4s)

[Limitations of the Internet](https://www.youtube.com/watch?v=R5aUp2KzG78&t=197s)


🔥 **IPv4 (Internet Protocol version 4): 32‑bit addresses, dotted‑decimal form**  
  - **Format:** 32 bits separated into four groups (dotted decimal).  
  - **Examples:** **73.55.242.3**, **172.14.24.1**.  
  - **Total possible:** **2^32 = 4,294,967,296 (~4.3 billion)** addresses.  
  - **Usable count is less** because some addresses are **reserved for special purposes** (reduces the pool available to devices).

💡 **IPv4 address scarcity and real‑world pressure**  
  - **Problem:** The number of devices worldwide has exceeded the pool of usable IPv4 addresses.  
  - **Consequence:** Alternative approaches are required to let more devices connect without unique public IPv4 addresses.

🚀 **IPv6 (Internet Protocol version 6): massively larger address space**  
  - **Format and size:** **128 bits** (four times the bit length of IPv4), typically represented as hexadecimal groups separated by colons.  
  - **Address space:** **2^128** possible addresses — an astronomically large number.  
  - **Analogy for scale:** Even the estimated **~7.5×10^18 grains of sand on Earth** would not be enough; you need the sand from multiple Earths to approach that number.  
  - **Implication:** **IPv6 supply is effectively inexhaustible** for foreseeable needs.
IPv6:
<img width="1274" height="301" alt="image" src="https://github.com/user-attachments/assets/42cb647b-1e38-4772-9487-27df0600267e" />


🔁 **Network Address Translation (NAT) as an IPv4 mitigation**  
  - **Function:** Allows one **public IP address** to be shared by many **private IP addresses** inside a local network.  
  - **Analogy:** NAT acts like a company receptionist who answers one public number and forwards callers to internal extensions.  
  - **Benefit:** Reduces the number of public IPv4 addresses an organization needs.

<img width="1270" height="446" alt="image" src="https://github.com/user-attachments/assets/99fadac6-cbee-45b8-8401-1db4a3f05b04" />


🛠 **Operational relevance for IT/support roles**  
  - **Task:** Configuring NAT on routers is a common duty to enable internal devices to communicate with the Internet using a shared public IP.  
  - **Context:** Routers are the point where NAT is implemented to bridge a company's private network and the outside world.

📈 **Adoption dynamics and coexistence**  
  - **Status:** **IPv6 adoption is slow but steady.**  
  - **Expectation:** IPv6 addresses will become increasingly common over time; until then, IPv4 + NAT and mixed deployments will persist.
