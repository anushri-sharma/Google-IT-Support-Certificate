
# Practice Quiz: Basic Commands

<img width="685" height="378" alt="image" src="https://github.com/user-attachments/assets/926fa05b-205f-424b-b834-b1e02d061118" />


```
Why this is correct:
    rm -r → required to delete directories
    \ → escapes the space so Bash treats it as a single name

❌ Incorrect options:
- rm Miscellaneous Directory
    - No -r flag → cannot remove directories
    - Also splits into two arguments (Miscellaneous and Directory) → wrong

- rm -r Miscellaneous Directory
    - Missing escaping or quotes → treated as two separate items → wrong

- rm Miscellaneous\ Directory
    - Missing -r → cannot remove directories → wrong

```

<img width="795" height="493" alt="image" src="https://github.com/user-attachments/assets/b6fbd3f9-7fef-4af4-b463-5cdc09a8f714" />

```
Explanation:
1. ls is the correct Bash command to list directory contents.
2. -l shows detailed (long) listing.
3. -a includes hidden files.
4 ./home specifies the directory.

Why the others are incorrect:
- list -a /home → ❌ list is not a valid Bash command.
- ls -la ~ → ⚠️ This lists the current user’s home directory (~), not /home.
```

<img width="842" height="517" alt="image" src="https://github.com/user-attachments/assets/d3c87106-8031-4ba3-9244-01404cf71eb8" />
<img width="694" height="266" alt="image" src="https://github.com/user-attachments/assets/80feb426-3b7c-485e-88be-398ed6790b42" />

```
Why these are correct:
- cd ../Alaska
  .. moves up one level from Canada to Pictures
  Then enters Alaska → ✔ valid relative path

- cd /home/cindy/Pictures/Alaska
   Absolute path from root → ✔ always works regardless of current location

❌ Incorrect options:

- ls ../Pictures/Alaska
  ls only lists files; it does not change directories → ❌

- cd /Pictures/Alaska
  This path is incorrect because /Pictures is not at the root level in the given tree → ❌
```

<img width="736" height="357" alt="image" src="https://github.com/user-attachments/assets/b48efbd1-9951-47b8-85c3-410f07c27aad" />

<img width="859" height="468" alt="image" src="https://github.com/user-attachments/assets/5ce6d70f-01f8-4df7-b20b-e7f14ed387e6" />

