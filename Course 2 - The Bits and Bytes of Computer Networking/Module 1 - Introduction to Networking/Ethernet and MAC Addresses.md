
# [Ethernet and MAC Addresses](https://www.youtube.com/watch?v=D1xpujHNkQc&t=8s)


🔥 Role of Ethernet and the data link layer  
  – **Ethernet** is the most widely used protocol for sending data across individual links, especially in workplaces and data centers.  
  – The **data link layer** abstracts the physical layer so higher layers (transport, application) can operate the same regardless of physical connection (e.g., twisted pair vs wireless).  
  – Learning objectives covered: explain **MAC addresses**, describe **Ethernet frame** components, differentiate **unicast/multicast/broadcast**, and explain **CRC** for data integrity.

📜 History and evolution  
  – Ethernet originated around **1980** and was first fully standardized in **1983**.  
  – Changes since then mainly address increasing bandwidth needs; core Ethernet concepts remain comparable to the original standard.

⚠️ Collision domains and why collisions matter  
  – A **collision domain** is a network segment where all devices receive all transmissions and only one device can successfully transmit at a time.  
  – Early LANs used hubs (no switches), so simultaneous transmissions caused literal collisions of electrical signals, producing unintelligible data.  
  – Because every node receives all traffic in a collision domain, addressing is required to indicate the intended recipient.

🔁 CSMA/CD (Carrier Sense Multiple Access with Collision Detection)  
  – **CSMA/CD** governs when a node can transmit: a node listens (carrier sense) and transmits only if the medium is idle.  
  – If two devices transmit simultaneously, they **detect the collision**, stop sending, and each waits a random backoff interval before retrying.  
  – The random backoff reduces the chance of repeated collisions among the same devices.

<img width="1280" height="409" alt="image" src="https://github.com/user-attachments/assets/d0b4377b-eb6d-4178-99b9-347b8c47c6f0" />


🆔 MAC address purpose and usage  
  – A **MAC address** (Media Access Control address) is a **globally unique identifier** attached to a network interface, used as source and destination addressing on Ethernet so nodes know which frames are meant for them.  
  – Ethernet frames include both **source** and **destination** MAC addresses to support communication on shared media.

<img width="1274" height="395" alt="image" src="https://github.com/user-attachments/assets/549b4e4f-43c6-469e-903b-d039ab2ddc07" />


🔢 MAC address format and numeric details  
  – A MAC address is **48 bits**, usually represented as **six groupings of two hexadecimal numbers** (e.g., XX:XX:XX:XX:XX:XX).  
  – Hexadecimal uses digits **0–9** and letters **A–F** to represent values **10–15**.  
  – An **octet** is 8 bits; two hexadecimal digits represent one octet.  
  – Total possible MAC addresses: **2^48 = 281,474,976,710,656**, providing a very large address space.

🏷️ MAC address allocation and the OUI  
  – The first **three octets** of a MAC address are the **Organizationally Unique Identifier (OUI)**, assigned to hardware manufacturers by the **IEEE**.  
  – The OUI allows identification of the manufacturer from the MAC address.  
  – The last **three octets** are assigned by the manufacturer in any scheme they choose, with the requirement that each assigned address be unique.



