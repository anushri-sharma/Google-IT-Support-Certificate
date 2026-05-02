
# Practice Quiz: Network Attacks

<img width="559" height="371" alt="image" src="https://github.com/user-attachments/assets/693868fe-4604-4ea2-9d65-5a26ff343bc0" />

```
Explanation:
A denial-of-service (DoS) attack overwhelms a system so legitimate users can’t access it. The main outcome is that the service becomes unavailable.

Why others are incorrect:

❌ Email address theft → relates to data breaches/phishing
❌ Malware infection → involves malicious software
❌ Data destruction → not the primary goal of DoS

Quick tip: DoS = deny access → service goes down.

```

<img width="586" height="395" alt="image" src="https://github.com/user-attachments/assets/d3b109a7-aef6-4020-9ed5-031a7a58adb2" />

```
Explanation:
The attacker is taking over an already authenticated session (using the active login token) without needing the password. This is exactly what session hijacking is.

Why others are incorrect:

❌ Rogue AP → involves fake Wi-Fi networks
❌ Trojan → malware disguised as legitimate software
❌ Ransomware → locks/encrypts data for payment

Quick tip: If someone “walks into an already logged-in session,” think session hijacking.
```


<img width="589" height="437" alt="image" src="https://github.com/user-attachments/assets/6b63c8c0-2a47-40d0-b840-3be50d536cc3" />

```

Explanation:
A DDoS (Distributed Denial-of-Service) attack uses many compromised systems (often a botnet) to flood a target with traffic, overwhelming it and making the service unavailable.

Why others are incorrect:

❌ Redirecting traffic → That’s more like DNS poisoning
❌ One source flooding → That’s a DoS, not distributed
❌ Stealing tokens → That’s session hijacking

Quick tip: DDoS = Distributed = many machines attacking at once.
```

<img width="661" height="501" alt="image" src="https://github.com/user-attachments/assets/476d920b-989f-45d7-a651-7bd6f1670991" />

```
Why this is a Rogue AP
A rogue access point is any wireless point installed on a network without the explicit authorization of the network administrator. In many cases, it isn't installed with "evil" intent; it’s often an employee trying to get better Wi-Fi in their office. However, because it bypasses the company's official security protocols (like firewalls or 802.1X authentication), it creates a wide-open back door for attackers.

Clarifying the Other Options
It is easy to mix these up because they all involve network deception. Here is a breakdown of what the other scenarios actually describe:

Evil Twin Attack: (The second option) This is very similar to a rogue AP, but the intent is different. In an Evil Twin attack, the attacker intentionally sets up a hotspot with the same name (SSID) as a legitimate network to trick people into connecting so they can steal credentials.

DoS/DDoS Attack: (The fourth option) Overloading a service with packets to make it unreachable is a Denial of Service attack.

Rootkit/Malware: (The first option) Modifying an operating system at the admin level usually describes a Rootkit or similar high-level malware infection.
```

<img width="875" height="383" alt="image" src="https://github.com/user-attachments/assets/0c635dbd-53d3-43be-9ab4-7c4b2b195b76" />


<img width="602" height="432" alt="image" src="https://github.com/user-attachments/assets/6b606792-3b16-42c5-9116-7f7db285cb1a" />

```
Explanation:
In a DNS cache poisoning attack, the attacker corrupts DNS records so that when you
try to visit a legitimate website, you’re silently redirected to a fake (malicious) one.
This can lead to phishing, malware downloads, or credential theft.

Why others are incorrect:

❌ It's not actually dangerous → It is very dangerous
❌ Access a site’s database → That’s more like SQL injection
❌ Remotely control your computer → That’s typically malware, not DNS poisoning

Quick tip: DNS poisoning = wrong address → wrong (malicious) website.

```


