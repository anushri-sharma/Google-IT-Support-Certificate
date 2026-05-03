# Graded Quiz: Module 4 challenge: Securing Your Networks


<img width="566" height="642" alt="image" src="https://github.com/user-attachments/assets/7859b823-bcc5-4c54-8682-927124b80a26" />

<img width="536" height="551" alt="image" src="https://github.com/user-attachments/assets/18cf652c-066e-477e-a5e6-82caaa920c1e" />

<img width="548" height="718" alt="image" src="https://github.com/user-attachments/assets/b22cf739-57dc-440e-94d3-168648bb81b9" />

<img width="517" height="563" alt="image" src="https://github.com/user-attachments/assets/05df352d-cd0c-4cc8-ade7-e3d04dff1b88" />

<img width="523" height="676" alt="image" src="https://github.com/user-attachments/assets/ebbdc313-a684-4624-a062-1adafb7360b8" />

<img width="513" height="545" alt="image" src="https://github.com/user-attachments/assets/daa04819-cd17-4021-af9f-02114e19756e" />

<img width="507" height="481" alt="image" src="https://github.com/user-attachments/assets/125a8d8b-a919-4e42-a176-3e586be983f7" />

<img width="537" height="706" alt="image" src="https://github.com/user-attachments/assets/010e6f85-727a-4338-ac59-985916c8eec4" />



1. What can protect your network from DoS attacks?
✅ Flood Guards
They limit excessive traffic to prevent denial-of-service conditions.

Flood guards are features on firewalls and enterprise switches designed to detect and block malicious traffic patterns, such as SYN floods or ICMP floods, by limiting the number of half-open connections or packets per second.

2. Which enterprise switch features protect against layer 2 man-in-the-middle attacks? (Select all that apply)
✅ Dynamic ARP inspection (DAI)
✅ IP Source Guard
✅ DHCP Snooping
❌ Flood Guard (used for DoS, not MITM)

Note: These three work together. DHCP Snooping builds a database of trusted IP/MAC pairings; DAI uses that database to prevent ARP spoofing; and IP Source Guard prevents IP spoofing by checking that the IP address in a packet matches the one assigned by DHCP.


3. A host-based firewall protects against malicious attacks in which scenarios? (Select all that apply)
✅ A device on a company’s internal network needs protection when another device connected to the network has been corrupted.
✅ An employee connects to the unsecured internet at their local coffee shop with their company computer.
❌ Rogue DHCP server attack
❌ Layer 2 MITM attack

4. What underlying symmetric encryption cipher does WEP use?
✅ RC4

WEP (Wired Equivalent Privacy) uses the RC4 stream cipher. It is considered highly insecure today because the small "Initialization Vector" (IV) it uses leads to key reuse, allowing attackers to crack the password in minutes.

5. What makes WPS PIN authentication vulnerable to brute force attacks?
✅ It uses an 8 digit PIN, which is made of 7 digits and one checksum value, and sends it in two parts. This means it takes a maximum of 11,000 tries to guess the PIN.

6. How can you increase the security of a WPA2 (AES/CCMP) wireless network?
✅ Use a long, complex passphrase that wouldn’t be found in the dictionary.

While WPA2-AES is strong, it is still vulnerable to "offline" brute force and dictionary attacks if the password is weak. Increasing length and complexity exponentially increases the time required to crack the handshake.

7. Technique to access all packets from a port, range, or VLAN?
✅ Port mirroring
(SPAN copies traffic to a monitoring system.)

Also known as SPAN (Switched Port Analyzer), port mirroring tells a switch to send a copy of all packets seen on one port (or VLAN) to another port where a monitoring device (like an IDS) is plugged in.

8. NIDS setup best practices? (Select all that apply)
✅ Use port mirroring to mirror all network traffic to the NIDS host.
✅ Set up the NIDS host with two network interfaces; one for analysis and one for management.
✅ Enable promiscuous mode on the NIDS analysis port.
❌ Set up the NIDS in-line (that’s IPS behavior)

9. Correct tcpdump command:
✅ sudo tcpdump -i eth0 -vn host 113.8.81.2 and port 8080 &


This command specifies the interface (-i eth0), enables verbose output (-v), disables name resolution for speed (-n), and filters for both the specific IP and the specific port. The & at the end runs it in the background.

10. Which flags should you use?
✅ -vn

-v gives useful detail
-n avoids DNS resolution (faster, cleaner output)


2. Which enterprise switch features protect against layer 2 man-in-the-middle attacks? Select all that apply.

Flood Guard

Dynamic ARP inspection (DAI)

IP Source Guard

DHCP Snooping

3. A host-based firewall protects against malicious attacks in which of the following scenarios? Select all that apply.

A device on a company’s internal network needs protection when another device connected to the network has been corrupted.

A company’s network experiences a rogue DHCP server attack.

A company’s network experiences a layer 2 man-in-the-middle attack.

An employee connects to the unsecured internet at their local coffee shop with their company computer.

4. What underlying symmetric encryption cipher does WEP use?
- AES
- RSA
- DES
- RC4

5. What makes the WPS method of PIN entry authentication with a hard-coded pin vulnerable to online brute force attacks?

- It uses an 8 digit PIN, which is made of 7 digits and one checksum value, and sends it in two parts. This means it takes a maximum of 11,000 tries to guess the PIN.
- There is a one-minute lockout period after three incorrect PIN attempts.
- It uses an 8 digit pin that is made of 7 digits and one checksum value. This means it takes a maximum of 10,000,000 tries to guess the PIN.
- It allows for the secure exchange of the SSID and the pre-shared key.


6. How can you increase the security of a wireless network that uses WPA2 with AES/CCMP mode?

Use a long, complex passphrase that wouldn’t be found in the dictionary.

Connect clients with SSID.

Connect clients with WPS.

Change the SSID to something rare and unique.


7. You’re an IT support specialist and you’ve been tasked with making sure the company is monitoring its network traffic adequately. What technique should you use if you want to access all packets from a specified port, port range, or entire VLAN?
- DHCP snooping
- Network hub
- tcpdump
- Port mirroring


8. You’re an IT support specialist tasked with setting up a NIDS system to monitor your company’s network traffic for suspicious behavior. Which of the following options would you implement? Select all that apply.

Use port mirroring to mirror all network traffic to the NIDS host.

Set up the NIDS in-line with all incoming traffic.

Set up the NIDS host with two network interfaces; one for analysis and one for management.

Enable promiscuous mode on the NIDS analysis port.


9. Complete the Qwiklab Introduction to tcpdump before answering this question.

You want to use tcpdump to retrieve packets with 113.8.81.2 as the source or destination IP address and port 8080 as the source or destination port. Which command should you use?

sudo tcpdump -i -vn host 113.8.81.2 and port 8080 &
sudo tcpdump -i eth0 -vn host 8.8.8.8 and port 8080 &
sudo tcpdump -i eth0 -vn host 113.8.81.2
sudo tcpdump -i eth0 -vn host 113.8.81.2 and port 8080 &


10. Complete the Qwiklab Introduction to tcpdump before answering this question.

You want to determine the layer 3 protocol, source, and destination addresses and ports for all incoming packets, as well as their TCP details. However, you don’t want more detailed output. What additional flags should you use with the command sudo tcpdump -i eth0?

1. -v
2. -n
3. -vn
4. none

   
