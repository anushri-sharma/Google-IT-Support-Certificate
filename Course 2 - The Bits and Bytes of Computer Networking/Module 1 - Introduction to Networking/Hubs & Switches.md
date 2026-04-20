
# [Hubs and Switches](https://www.youtube.com/watch?v=2z7yyhDlmAI&t=3s)


**Cables** allow you to form point to point networking connections.

These are networks where only a single device at each end of the link exists.

Not to knock point to point networking connections, but they're not super useful in a world with billions of computers.

Luckily, there are network devices that allow for many computers to communicate with each other.

The most simple of these devices is a **hub**.

<img width="1269" height="403" alt="image" src="https://github.com/user-attachments/assets/db0b55c9-611a-4d19-a277-4e9e697d27e5" />


**A hub is a physical layer device** that allows for connections from many computers at once.

<img width="1272" height="588" alt="image" src="https://github.com/user-attachments/assets/02b31069-5c8c-4078-bbd9-504c7db6f821" />


All the devices connected to a hub will end up talking to all other devices at the same time.

It's up to each system connected to the hub to determine if the incoming data was meant for them or 
to ignore it if it isn't.

This causes a lot of noise on the network and creates what's called a collision domain.

A **collision domain** is a network segment where only one device can communicate at a time.

<img width="1272" height="412" alt="image" src="https://github.com/user-attachments/assets/9a3823c9-1dfe-4f61-ba86-1fe311356962" />

<img width="1277" height="359" alt="image" src="https://github.com/user-attachments/assets/bf592715-5e88-4bf5-ac3b-0c9b50943ff7" />

<img width="1269" height="656" alt="image" src="https://github.com/user-attachments/assets/3fa60201-7038-4b26-a5db-0720e76063a1" />


If multiple systems try sending data at the same time, the electrical pulses sent across the cable can 
interfere with each other.
This causes these systems to have to wait for a quiet period before they try sending their data again.

It really slows down network communications and is the primary reason hubs are fairly rare, they're mostly 
a historical artifact today.

**A much more common way of connecting many computers is with a more sophisticated device known as a network 
switch**, originally known as a switching hub.

A **switch** is very similar to a hub since you can connect many devices to it so they can communicate.

<img width="1268" height="665" alt="image" src="https://github.com/user-attachments/assets/41787150-0b17-4fdf-ab6d-773e1db54f51" />

The **difference** is that while a **hub is a Layer 1** or physical layer device, a **switch is a Layer 2** or datalink device.

<img width="1280" height="554" alt="image" src="https://github.com/user-attachments/assets/dae3ccab-210a-4c8a-9724-a352afaca2c7" />

This means that a switch can actually inspect the contents of the Ethernet protocol data being sent around the
network, determine which system the data is intended for, and then only send that data to that one system.

This reduces or even completely eliminates the size of collision domains on a network.

<img width="1278" height="606" alt="image" src="https://github.com/user-attachments/assets/e40f92c4-3ac7-4482-9e5d-6d837dba8324" />


If you guess that this will lead to fewer retransmissions and a higher overall throughput.

<img width="1275" height="477" alt="image" src="https://github.com/user-attachments/assets/9feeb632-f599-4e2f-8b0f-3ca9acc5ff32" />


