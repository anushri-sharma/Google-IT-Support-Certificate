
# Practice Quiz: Verifying Connectivity


<img width="688" height="362" alt="image" src="https://github.com/user-attachments/assets/c96cba59-d8b2-42ad-930a-ec7fc4000ba0" />

```
✅ Test-NetConnection

This PowerShell command can check connectivity to a specific port
(e.g., Test-NetConnection google.com -Port 80).
❌ ping and tracert don’t test ports
❌ nc (netcat) is typically Linux-based, not native to Windows
```

<img width="702" height="412" alt="image" src="https://github.com/user-attachments/assets/e4281cb3-de54-4e0f-9a58-bcd80529fb00" />

```
On Linux and macOS, traceroute uses UDP packets by default
❌ Windows (tracert) uses ICMP, not UDP
```

<img width="675" height="315" alt="image" src="https://github.com/user-attachments/assets/9e7ef195-db51-4ac5-98d4-d0fa84ae5ac7" />

```
ping sends an ICMP Echo Request and receives an Echo Reply
```

<img width="640" height="335" alt="image" src="https://github.com/user-attachments/assets/39dfc2e3-f644-402d-9cfa-8e13b9b468b8" />

```
✅ ICMP (Internet Control Message Protocol)

Handles error messages and diagnostic functions (used by ping, traceroute)
```

<img width="703" height="338" alt="image" src="https://github.com/user-attachments/assets/510ca31b-f4f5-4bcb-8dee-f66b0cb4abce" />

```
✅ Subtraction

Each router decrements (subtracts 1) from the TTL value
When TTL reaches 0, the router sends an ICMP response
```
