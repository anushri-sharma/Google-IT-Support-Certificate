
# [Ethernet and MAC Addresses](https://www.youtube.com/watch?v=D1xpujHNkQc&t=8s)


🔥 Role of Ethernet and the data link layer  
  – **Ethernet** is the most widely used protocol for sending data across individual links, especially in workplaces and data centers.  
  – The **data link layer** abstracts the physical layer so higher layers (transport, application) can operate the same regardless of physical connection (e.g., twisted pair vs wireless).  
  – Learning objectives covered: explain **MAC addresses**, describe **Ethernet frame** components, differentiate **unicast/multicast/broadcast**, and explain **CRC** for data integrity.

<img width="1280" height="299" alt="image" src="https://github.com/user-attachments/assets/bcc69c84-0ff9-4d30-98fc-f7196f5e03bf" />


📜 History and evolution  
  – Ethernet originated around **1980** and was first fully standardized in **1983**.  
  – Changes since then mainly address increasing bandwidth needs; core Ethernet concepts remain comparable to the original standard.

⚠️ Collision domains and why collisions matter  
  – A **collision domain** is a network segment where all devices receive all transmissions and only one device can successfully transmit at a time.  
  – Early LANs used hubs (no switches), so simultaneous transmissions caused literal collisions of electrical signals, producing unintelligible data.  
  – Because every node receives all traffic in a collision domain, addressing is required to indicate the intended recipient.

🔁 CSMA/CD (Carrier Sense Multiple Access with Collision Detection)  
  – **CSMA/CD** governs when a node can transmit: a node listens (carrier sense) and transmits only if the medium is idle.  

<img width="1278" height="455" alt="image" src="https://github.com/user-attachments/assets/28c1ad2a-fe77-4b33-9970-5f8d638a11f6" />

  
  – If two devices transmit simultaneously, they **detect the collision**, stop sending, and each waits a random backoff interval before retrying. 

 <img width="1280" height="327" alt="image" src="https://github.com/user-attachments/assets/808cfbaa-84f8-4103-8df1-c28561cfa216" />
 
  – The random backoff reduces the chance of repeated collisions among the same devices.

- **When a network segment is a collision domain**, it means that all devices on that segment receive all communication across the entire segment.

- This means we need a way to identify which node the transmission was actually meant for.

- This is where something known as a **Media Access Control address or Mac address** comes into play.

🆔 MAC address purpose and usage  
  – A **MAC address** (Media Access Control address) is a **globally unique identifier** attached to a network interface, used as source and destination addressing on Ethernet so nodes know which frames are meant for them.  
  – Ethernet frames include both **source** and **destination** MAC addresses to support communication on shared media.

<img width="1274" height="395" alt="image" src="https://github.com/user-attachments/assets/549b4e4f-43c6-469e-903b-d039ab2ddc07" />


🔢 MAC address format and numeric details  
  – A MAC address is **48 bits**, usually represented as **six groupings of two hexadecimal numbers** (e.g., XX:XX:XX:XX:XX:XX).  
  – Hexadecimal uses digits **0–9** and letters **A–F** to represent values **10–15**.  
  – An **octet** is 8 bits; two hexadecimal digits represent one octet.  

<img width="1277" height="367" alt="image" src="https://github.com/user-attachments/assets/8872a2f4-18a1-4cf0-923c-493802a49fcf" />
  
  – Total possible MAC addresses: **2^48 = 281,474,976,710,656**, providing a very large address space.

<img width="1275" height="272" alt="image" src="https://github.com/user-attachments/assets/611a4a29-12b7-4651-9a9f-227e5459a92f" />


🏷️ MAC address allocation and the OUI  

<img width="1279" height="321" alt="image" src="https://github.com/user-attachments/assets/7bd18b54-b972-493f-9a84-3c0ccc915479" />

**A MAC address is split into two sections**.

  – The first **three octets** of a MAC address are the **Organizationally Unique Identifier (OUI)**, assigned to hardware manufacturers by the **IEEE**.  
  – The OUI allows identification of the manufacturer from the MAC address. 
  _ This is a useful bit of information to keep in your back pocket, because it means that you can always identify the manufacturer of a network interface purely by its Mac address.

<img width="1246" height="574" alt="image" src="https://github.com/user-attachments/assets/55490e42-5588-438c-98bf-6f0114c42270" />
  
  – The last **three octets** are assigned by the manufacturer in any scheme they choose, with the requirement that each assigned address be unique.

<img width="1244" height="566" alt="image" src="https://github.com/user-attachments/assets/6e2d208e-b9ec-4587-8b84-5e6b9d32f446" />


<img width="1280" height="377" alt="image" src="https://github.com/user-attachments/assets/0af3bd18-2fdd-4880-946f-4a3e0ce8b83b" />






