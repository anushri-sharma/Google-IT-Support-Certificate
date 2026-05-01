
# Practice Quiz: Centralized Management and LDAP


<img width="568" height="703" alt="image" src="https://github.com/user-attachments/assets/3643b98c-cbf2-4f72-b43c-045534b043d2" />

<img width="574" height="520" alt="image" src="https://github.com/user-attachments/assets/93d6f7b6-97f8-4068-b93f-cb61fce28fb0" />

```
1. Centralized Authentication

This is the primary function of a Directory Service. Instead of managing user credentials
on every individual machine, a Directory Service allows users to log in once to a central
system. This "single source of truth" verifies the user's identity across the entire network.

2. Authorization

Once a user is authenticated, the Directory Service helps manage Authorization. It defines
what resources a user can access (e.g., specific folders, printers, or applications) based
on their role or group membership.

3. Accounting

Directory Services often handle the "AAA" framework (Authentication, Authorization, and
Accounting). Accounting involves tracking what a user does while they are logged in, including
resource usage and session duration, which is vital for security audits and compliance.

Why "Local Authentication" is excluded:
While individual computers perform local authentication for users not on a network, Directory Services are specifically built to replace or bypass local authentication in favor of a centralized model. This ensures consistency and security across many different devices.


```

<img width="525" height="436" alt="image" src="https://github.com/user-attachments/assets/1bdb5351-6174-451b-b4b8-e05c734dea8a" />

```
Explanation:
LDAP Bind supports:

Simple → username/password authentication
SASL → more advanced, flexible authentication methods
Anonymous → no credentials required (limited access)

“Complex” isn’t an official LDAP bind method.

```

<img width="509" height="579" alt="image" src="https://github.com/user-attachments/assets/c7cdf464-2b3c-42f3-bab2-a8d734746ed3" />

<img width="535" height="634" alt="image" src="https://github.com/user-attachments/assets/f62d6eef-5814-4def-a8ce-76a95daea5b3" />
<img width="466" height="352" alt="image" src="https://github.com/user-attachments/assets/3b71af74-0864-4c79-978b-28b04c1a2d6f" />

