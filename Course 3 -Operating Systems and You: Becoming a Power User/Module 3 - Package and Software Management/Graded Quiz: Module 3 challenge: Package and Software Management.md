
# Graded Quiz: Module 3 challenge: Package and Software Management



<img width="731" height="362" alt="image" src="https://github.com/user-attachments/assets/fe369650-48e6-43a9-bf15-a4adb1c2c0bb" />

```

Explanation:

The Microsoft Store uses APPX (and newer MSIX) package formats to distribute
Universal Windows Platform (UWP) apps. These packages are designed specifically
for secure installation, sandboxing, and easy updates.

Why others are incorrect:
❌ Windows executable files (.exe) → Traditional desktop apps, not Store apps
❌ Microsoft install packages (.msi) → Used for enterprise/traditional software installs
❌ Debian packages (.deb) → Used in Linux systems like Ubuntu
```


<img width="713" height="338" alt="image" src="https://github.com/user-attachments/assets/2c6e09e5-e13f-4af8-b8a7-ba73fc61f352" />

```

Explanation:

1. The command dpkg -i is used in Ubuntu (and other Debian-based systems)
to install a .deb package file.

2. -i stands for install.

3. So, dpkg -i UbuTestPackage means you are installing that package manually
(assuming it's a .deb file like UbuTestPackage.deb).

Why the others are incorrect:
❌ Uninstall → uses dpkg -r
❌ Search → uses tools like dpkg -l or apt search
❌ Uninstall DPKG → unrelated and incorrect

```

<img width="698" height="332" alt="image" src="https://github.com/user-attachments/assets/38a36706-ef12-435d-b9b8-5891a5dccf56" />

```
Explanation:

Side-loading is the process of installing an app on a mobile OS from outside the
official app store (like installing an APK file directly on Android instead of
using the Play Store).

Why others are incorrect:
❌ Unlocking → Refers to removing restrictions (like carrier locks), not installing apps
❌ Down-storing → Not a real term
❌ Uploading → Sending data to a server, not installing apps

👉 So remember: Installing apps from unofficial sources = Side-loading

```


<img width="670" height="339" alt="image" src="https://github.com/user-attachments/assets/5a201fb4-bc78-4f05-9e93-9c05201cf8e3" />

```
In PowerShell, the Compress-Archive cmdlet is used to create a ZIP file from files or folders.

-Path → specifies the folder/files to compress
Destination (~\Desktop\TestArchive.zip) → where the ZIP file will be created

Why others are incorrect:
❌ Create-Archive → Not a valid PowerShell cmdlet
❌ Expand-Archive → Used to extract ZIP files, not create them
❌ Archive → Not a valid cmdlet

👉 Easy way to remember:

Compress-Archive = create ZIP
Expand-Archive = extract ZIP
```

<img width="746" height="329" alt="image" src="https://github.com/user-attachments/assets/7278d4a5-068e-44d8-9575-a2c1edc30b95" />


<img width="635" height="287" alt="image" src="https://github.com/user-attachments/assets/25ed8f07-406a-4925-8e11-126a8f1965a0" />

```
A software repository is a centralized server or system where software packages are stored,
maintained, and distributed. Operating systems and package managers pull software from these
repositories when you install or update programs.

For example, in Linux distributions like Ubuntu, tools like APT download packages from
online repositories.

Why others are incorrect:
❌ A package manager used in Windows → That would be tools like Winget, not a repository
❌ An open-source graphical editor → Completely unrelated
❌ A package manager used in Ubuntu → That refers to APT, not the repository itself

👉 Simple idea:
Repository = storage place
Package manager = tool that fetches from it

```

<img width="759" height="354" alt="image" src="https://github.com/user-attachments/assets/2cfabe82-9686-4076-9b3f-a940d23aeda9" />

```
In Ubuntu (and Linux systems in general), device files in /dev represent hardware.

Files like /dev/sda, /dev/sdb, /dev/sdc refer to storage devices (hard drives, SSDs, USB drives).
The letters (a, b, c) indicate the order in which the system detects them.

So:

/dev/sdc is typically a third storage device, commonly a USB flash drive (memory stick) when plugged in.

Why others are incorrect:

❌ Monitor → Managed by display systems, not as /dev/sdX
❌ Printer → Usually appears as /dev/usb/... or via printer services
❌ Keyboard → Appears under input devices like /dev/input/...

👉 Quick tip:
/dev/sdX = storage devices (disks, USB drives)
```

<img width="748" height="401" alt="image" src="https://github.com/user-attachments/assets/771476c9-85cc-4c0f-be1d-8d804fd4944f" />


<img width="713" height="334" alt="image" src="https://github.com/user-attachments/assets/aa4de0bc-ae6a-4d25-93cc-4a202fd135c4" />

```

In Ubuntu (and most Linux systems), storage devices follow this naming pattern:

/dev/sda → first detected storage device
/dev/sdb → second
/dev/sdc → third

The letters (a, b, c, …) indicate the order in which the system detects the drives.

Why others are incorrect:
❌ /dev/sd0 and /dev/sd1 → Not valid naming convention in Linux
❌ /dev/sdc → Third device, not the first

👉 Easy memory trick:
“a = first, b = second, c = third”
```


<img width="713" height="348" alt="image" src="https://github.com/user-attachments/assets/20858335-9e95-4f41-8795-22ee0aaefe6d" />

```

Explanation:

In Ubuntu, the command:

sudo apt full-upgrade upgrades all installed packages and allows installing/removing dependencies if needed.
This is important for Linux kernel updates, since they often require adding or removing packages.
Why others are incorrect:
❌ sudo apt update → Only refreshes package lists, does NOT install updates
❌ install NewKernel → Not a valid command
❌ uname -r → Displays the current kernel version, does NOT update it

👉 Quick tip:

update = refresh list
upgrade = upgrade packages (no major changes)
full-upgrade = upgrade + handle dependencies (kernel updates possible)

```
