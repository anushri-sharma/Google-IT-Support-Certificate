# Graded Quiz: Module 4 challenge: Filesystems


<img width="697" height="338" alt="image" src="https://github.com/user-attachments/assets/1e57c68f-13c3-4cb1-a41d-6b73eabd2aed" />


<img width="639" height="278" alt="image" src="https://github.com/user-attachments/assets/fd86c629-0e5f-4a66-af66-641f5a1ce071" />

<img width="837" height="463" alt="image" src="https://github.com/user-attachments/assets/b1bef4b0-7240-40d8-9880-6f65a183f5e6" />

<img width="791" height="438" alt="image" src="https://github.com/user-attachments/assets/2603585a-de9a-489b-8c73-eca12663e994" />

<img width="691" height="346" alt="image" src="https://github.com/user-attachments/assets/ef1fadfc-bc60-42b9-b7f1-f168a132c397" />

<img width="681" height="301" alt="image" src="https://github.com/user-attachments/assets/83ed707c-420a-4fe9-aa02-6cc8cbef0d1b" />

<img width="723" height="331" alt="image" src="https://github.com/user-attachments/assets/8de59b96-d808-49c3-9c25-c03df2c3cbb5" />

<img width="697" height="306" alt="image" src="https://github.com/user-attachments/assets/2e476db6-7dbc-4d62-b576-899f055db9c5" />

<img width="731" height="315" alt="image" src="https://github.com/user-attachments/assets/9207498a-d95d-49c6-815e-923ea3a7fdd3" />

<img width="708" height="354" alt="image" src="https://github.com/user-attachments/assets/9edf3fbc-bad0-4e8e-abfe-1b285705e069" />



```
The partition table is the part of a disk that tells the operating system:

- How the disk is divided (partitions)
- Where each partition starts and ends
- What type of partition it is

Common partition table types:

- MBR (older)
- GPT (modern)

❌ Why others are wrong:

- The swap table → related to memory, not disk layout
- The master partition list → not a real standard term
- The filesystems grid → not a real concept

```


```

💡 Explanation:

These are partition table schemes—they define how a disk is divided and organized.

- MBR (Master Boot Record) → older partitioning scheme (limited to ~2TB, fewer partitions)
- GPT (GUID Partition Table) → modern scheme (supports large disks, many partitions)

❌ Why others are wrong:

- NTFS (New Technology File System) → this is a filesystem, not a partition table
- UEFI (Unified Extensible Firmware Interface) → this is firmware used for booting, not partitioning

```


```
💡 Explanation:

When you enable compression:

Data is stored in a compressed format, so
  👉 ✔ It uses less disk space

When you open a file, the system automatically decompresses it, so
  👉 ✔ Files need to be expanded when opened

❌ Why the others are wrong:

❌ The formatting process will complete in less time
  → Compression adds extra work → may take longer

❌ The computer's processor will need to do less work
  → Compression/decompression requires more CPU effort

```


```
💡 Explanation:

When you run sudo parted -l in Linux:

- It lists all disks and their partition tables (e.g., MBR, GPT)
- It shows each partition on the disk → so you can count them
- It displays partition sizes and disk sizes

❌ Why this is wrong:

❌ The security permissions for each partition
→ parted does NOT show permissions
→ Permissions are handled by filesystem tools like ls -l
🎯 Final Tip

👉 parted -l = disk + partition structure info, not file permissions
```


```
💡 Explanation:

The Windows Memory Manager is responsible for handling how memory is used:

✔ It maps virtual memory to physical RAM so programs can run efficiently
✔ It uses techniques like paging to load data into memory only when needed

❌ Why others are wrong:

❌ Format and partition memory
  → That’s related to disks, not RAM

❌ Stores the user's favorite photo memories in a virtual album
  → Not a real function (just a trick option)
🎯 Final Concept

👉 Memory Manager = efficient use of RAM + virtual memory handling

```


```
💡 Explanation:

A swap file / swap space is used by the operating system when RAM is full:

- It acts as extra memory on disk
- Stores inactive data from RAM
- Helps run more programs than physical memory allows

❌ Why others are wrong:

❌ A file that acts as a drive partition → not correct
❌ An online forum for swapping files → unrelated
❌ An Exchange file → not a real concept here

🎯 Final Concept

👉 Swap space = backup memory on disk when RAM is insufficient

```

```
💡 Explanation:

In the NTFS filesystem, the Master File Table (MFT) stores information about every file.

- Each file has a unique file record number (FRN)
- This number is used to index and locate the file’s entry in the MFT

❌ Why others are wrong:

❌ The volume → refers to the disk/partition, not a file identifier
❌ The creation timestamp → just metadata, not an index
❌ The filename → names can change; indexing uses a unique number
🎯 Final Concept

👉 MFT uses file record numbers (FRN) to track files internally

```

```
💡 Explanation:

In Linux:

- A hardlink points directly to the file’s inode (index node)
- The inode contains the file’s actual data location and metadata
- So both the original file and the hardlink point to the same underlying data

❌ Why others are wrong:

❌ By referencing a copy of the other file
  → Hardlinks do NOT create a copy
❌ By referencing the other file's name
  → That’s how symbolic links (symlinks) work
❌ By referencing the other file's physical location on the hard drive
  → The filesystem manages location via the inode, not directly exposed

🎯 Final Concept

👉 Hardlink = same inode, same data, different filename

```


```
💡 Explanation:
chkdsk (Check Disk) is the Windows utility used to:
Scan the file system for errors
Fix issues when used with options like /f

👉 Example:

- chkdsk /f

❌ Why others are wrong:

❌ fsck → Linux disk check tool
❌ chkfix → not a real command
❌ chkdsk (with space) → not a valid command format

🎯 Final Concept

👉 Windows = chkdsk
👉 Linux = fsck

```

```
💡 Explanation:

In Linux, the filesystem keeps a status flag (dirty bit) in its metadata.

- If the system shuts down improperly or detects issues
- This flag is set → indicating possible corruption
- On next boot, the system automatically runs fsck to check and repair

❌ Why others are wrong:

❌ At whatever time you schedule your system to run fsck
→ That’s manual scheduling, not automatic behavior
❌ Any time you boot your computer
→ fsck does NOT run every boot (only when needed)
❌ Only when you update your Linux kernel
→ No relation to filesystem checks

🎯 Final Concept

👉 Linux runs fsck automatically only when filesystem inconsistency is detected

```

