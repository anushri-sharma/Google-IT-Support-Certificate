
# Practice Quiz: Dynamic Host Configuration Protocol


<img width="862" height="548" alt="image" src="https://github.com/user-attachments/assets/d0ac52b0-9895-486d-bcd7-92de00b3540f" />

```
IP address → Identifies the device on the network (like a home address)

Name server (DNS) → Converts domain names (like google.com) into IP addresses
```

<img width="850" height="603" alt="image" src="https://github.com/user-attachments/assets/5940124a-aad6-4c83-903a-d9353e8527ce" />

```
ANS 2:

When a client is set to use DHCP, it follows a process called DORA:

- Discovery → Client broadcasts: “Any DHCP server available?”
- Offer → Server offers an IP address
- Request → Client requests that offered IP
- Acknowledgement → Server confirms and assigns it

```

```
ANS 3:

DHCP (Dynamic Host Configuration Protocol) works at the Application Layer of the OSI model.

It provides services like assigning:
- IP address
- Subnet mask
- Default gateway

It uses lower-layer protocols:
  1. UDP (Transport layer)
  2. IP (Network layer)

```

<img width="696" height="335" alt="image" src="https://github.com/user-attachments/assets/49dbfc8c-a456-4f9d-b471-59b2bbc92158" />

```
In Fixed Allocation DHCP (also called DHCP reservation):

- The DHCP server assigns a specific IP address to a device
- It identifies the device using its MAC address (unique hardware ID)

So every time that device connects, it gets the same IP
```

<img width="720" height="448" alt="image" src="https://github.com/user-attachments/assets/2c7a7c92-098b-4634-b646-e6ab9905662f" />


```
DHCP can operate in different ways:

Dynamic allocation → IPs are assigned temporarily from a pool
Fixed allocation (reservation) → Same IP is always assigned to a device based on its MAC address

❌ Incorrect options:
ARP ✖️ → Used for mapping IP to MAC addresses, not a DHCP mode
CIDR ✖️ → Used for IP address allocation/routing, not DHCP operation

```
