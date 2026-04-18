[BIOS](https://www.youtube.com/watch?v=W36kZakFm_Q)

🔥 **How external devices reach the CPU: drivers/services**  
  – **Devices (keyboard, mouse, webcam, printers)** send raw data that the CPU cannot interpret alone (for example, a keypress is just a byte).  
  – **Drivers (services)** are programs that contain the instructions the CPU needs to understand and control these devices.  
  – **Drivers are typically loaded by the operating system** from persistent storage (hard drive) once the OS is running.

💡 **BIOS/firmware role in startup**  
  – **BIOS (Basic Input/Output System)** is firmware that helps initialize hardware and starts the operating system.  
  – **BIOS runs before the OS** and provides the low-level interface needed for the system to boot and to discover hardware.

<img width="1268" height="455" alt="image" src="https://github.com/user-attachments/assets/f0c096a4-6224-48de-87b0-df299ede7503" />

<img width="1157" height="554" alt="image" src="https://github.com/user-attachments/assets/8336dee1-813e-4675-804e-05d631c997e8" />


🧾 **Where BIOS lives (non-volatile storage)**  
  – BIOS is stored on the **motherboard in non-volatile memory (ROM/flash)**, not on the hard drive, so it persists when powered off.  
  – Unlike RAM, this memory **does not erase when the computer is turned off**.

🚀 **UEFI: modern replacement for traditional BIOS**  
  – **UEFI (Unified Extensible Firmware Interface)** performs the same startup function as BIOS but with improved compatibility and support for newer hardware.  
  – **Most modern hardware ships with UEFI**, and UEFI is progressively replacing legacy BIOS.

<img width="1278" height="556" alt="image" src="https://github.com/user-attachments/assets/da266b45-d656-409c-9e4b-e86d38944570" />


🔊 **POST (Power-On Self-Test) and beep codes**  
  – **POST is an early hardware self-test that runs at boot** to detect present hardware and basic faults, occurring before OS-level drivers are loaded.  
  – If video/display drivers are not yet available, **errors are often signaled by speaker beeps (beep codes)** rather than on-screen messages.  
  – **Beep codes vary by manufacturer**; a single beep commonly indicates success while multiple beeps can indicate specific POST errors—consult the motherboard manual for exact meanings.  
  – **Not all machines include a built-in speaker**, so absence of beep does not necessarily indicate success or failure.

⚙️ **CMOS and BIOS settings (configuration storage)**  
  – A separate, battery-backed memory area commonly called **CMOS** stores BIOS configuration like **date/time and boot order**.  
  – These settings can be changed from the **BIOS/UEFI settings menu** (accessed by pressing the indicated key during the brief boot screen).

CMOS:
<img width="1278" height="542" alt="image" src="https://github.com/user-attachments/assets/fef3a88c-aefc-47ee-97e2-7cd80514c553" />

🛠️ **Accessing and changing BIOS settings**  
  – Most systems show a **brief prompt during boot** that indicates which key to press to enter the BIOS/UEFI settings menu.  
  – In an IT support role, **modifying BIOS/UEFI settings is common**—for instance to change the boot device order.

💽 **Reimaging computers (why BIOS settings matter for IT tasks)**  
  – **Reimaging** means wiping a machine and installing a **disk image** (a copy of an operating system).  
  – Reimaging tools are often stored on **external media** (USB stick, CD-ROM) or on a **network server**.  
  – To boot from these external sources, you must **use BIOS/UEFI to set the boot priority** to the external device or network.


<img width="1277" height="327" alt="image" src="https://github.com/user-attachments/assets/e903854c-4f5b-49b7-b69c-1213dfbe3cb2" />

<img width="1280" height="352" alt="image" src="https://github.com/user-attachments/assets/35445020-c0f8-4322-bc48-60da7280305d" />



🧭 Practical troubleshooting and implications for IT support  
  – **Beep codes and POST behavior are valuable troubleshooting tools** when screen output is unavailable.  
  – **Knowing how to enter BIOS/UEFI and change boot order** is essential for tasks like OS installation, reimaging, and hardware diagnostics.  
  – **UEFI vs legacy BIOS differences** can affect boot media compatibility (e.g., UEFI-secure-boot settings), so confirm firmware mode when preparing bootable media.
