# Graded Quiz: Module 2 challenge: Users, Administrators, Groups and Permissions


<img width="679" height="305" alt="image" src="https://github.com/user-attachments/assets/a3a3a2ef-ec23-4b7a-af74-5cb468daf207" />

```
A standard user can:

Use applications
Access files
Perform everyday tasks

But has limited control (cannot install system-wide software or change critical settings without admin rights).

❌ Why others are incorrect:
Administrator → full control over the system
General → not a standard user type
Limited → informal term, not the correct classification
```

<img width="695" height="349" alt="image" src="https://github.com/user-attachments/assets/d2393d3e-e4d2-4f38-8a99-3c5cbd4cd154" />

```
✅ Correct answer: User must change password at next logon.

Why:

This setting forces the user to immediately update their password the next time they
sign in—ideal if the current password may be compromised.
```

<img width="672" height="304" alt="image" src="https://github.com/user-attachments/assets/0ed9ac1f-d5b4-4577-a592-be682efd0529" />


```
Why:
Get-LocalGroup lists all the local groups on a Windows computer.
❌ Why others are incorrect:
Get-GPOReport → generates Group Policy reports, not local groups
Get-LocalGroupMember → shows members inside a specific group
Get-LocalUser → lists local user accounts, not groups

```

<img width="660" height="317" alt="image" src="https://github.com/user-attachments/assets/9b3cbe6e-57cd-4936-abd0-23a020f879c6" />

```
/etc/passwd stores essential information about user accounts, such as:

- username
- user ID (UID)
- group ID (GID)
- home directory
- default shell

❌ Why others are incorrect:

/etc/group → stores group information
/etc/sudoers → defines sudo (admin) privileges
/etc/users → not a standard Linux file
```

<img width="689" height="318" alt="image" src="https://github.com/user-attachments/assets/59801875-d166-4657-989c-4850f0956b15" />

```
The net command is used in Windows CLI to manage users, including changing passwords.

Example:

net user username newpassword

❌ Why others are incorrect:

user command → not a valid Windows CLI command
new command → not used for user management
password command → not a standard Windows command

```


<img width="726" height="393" alt="image" src="https://github.com/user-attachments/assets/145acb51-9003-4237-8aab-f0d6147b7376" />


<img width="815" height="456" alt="image" src="https://github.com/user-attachments/assets/967e714a-18c4-4b80-b257-937aa636165a" />


<img width="787" height="437" alt="image" src="https://github.com/user-attachments/assets/4c4267a6-ef22-4b27-9eea-f83db7624510" />

```

8.
These are standard Windows NTFS permissions that can be assigned to users or groups:

List folder contents → view files/subfolders inside a directory
Write → create or modify files
Read & Execute → read files and run executable files

```

<img width="761" height="408" alt="image" src="https://github.com/user-attachments/assets/381ede02-0439-4d44-b921-76319f92c43e" />

```
The first character - → indicates a regular file (not a directory)
The next three characters rwx → owner permissions:
r = read
w = write
x = execute

So -rwx = regular file with full permissions for the owner ✔️

❌ Why others are incorrect:
Directory file → would start with d, not -
No execute permission → incorrect because x is present
Exchange permissions → not a valid Linux permission term
```

<img width="710" height="386" alt="image" src="https://github.com/user-attachments/assets/f8e668d0-bb37-4c84-bcc6-d52a2591a4a1" />


```
In Windows, simple permissions (like Read, Write, Modify, Full Control) are actually
combinations of more granular “special permissions.”

❌ Why others are incorrect:
admin permissions → not a defined category
user permissions → too generic
partial permissions → not a standard term

```
