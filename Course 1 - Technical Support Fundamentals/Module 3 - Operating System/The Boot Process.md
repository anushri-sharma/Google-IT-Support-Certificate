[The Boot Process](https://www.youtube.com/watch?v=YwcZi8Wy7yo)


It's important to know the steps and operating system takes, so you can help diagnose the issue.

Booting a computer or starting a computer comes from the phrase to pull oneself up by one's bootstraps.

Basically, it means to start from nothing and follow a series of steps to arrive at a fully operational system.

When we start up with computer, will use the term **boot**.

For most operating systems, the boot process follows a general pattern, much like how we have different cars startup in the same way.

Put in the key, turn on the ignition, etc.

Here's a rundown of the boot process.

First, the computer is powered on.

The **BIOS/UEFI** is a **low-level software that initializes our computer's hardware to make sure everything is good to go.**

<img width="1280" height="445" alt="image" src="https://github.com/user-attachments/assets/70ccc1db-9e13-468a-8e64-3455d5ac0803" />

Next, the bios UEFI runs a process called the power-on self-test, or post.

The post performs a series of diagnostic tests to make sure that the computer is in proper working order.

Next, depending on the bios or UEFI configuration of boot device will be selected.

<img width="1277" height="338" alt="image" src="https://github.com/user-attachments/assets/cff660c1-ee5c-4e9e-9f88-f1caaf1bb7c8" />

Devices that are attached to our system, like hard drives, USB drives, CD drives, etc, are configured in a certain boot order.

**The devices will be checked in this order and the computer will search for what's known as a bootloader.**

<img width="1280" height="474" alt="image" src="https://github.com/user-attachments/assets/98fbdf1c-a82c-4882-bbbe-2b093828e168" />

**The bootloader is a small program that loads the operating system.**

Once our computer finds a bootloader on a device in the listed order, it will start to execute this program.

This will then start to load a larger and more complex program and eventually loads our operating system.

<img width="1278" height="532" alt="image" src="https://github.com/user-attachments/assets/61198f3a-9fea-4e8d-8420-f5ecfb8998c7" />

Once the **bootloader loads** up our **operating system, our kernel gets loaded**.

<img width="1278" height="610" alt="image" src="https://github.com/user-attachments/assets/8ee82b67-5d64-46e3-9da3-0876be815953" />

The **kernel controls** access to our computer's resources.

<img width="1110" height="632" alt="image" src="https://github.com/user-attachments/assets/3ec438e3-0b1c-4311-a4f8-ad6bda386baf" />

It also loads up drivers and more so that our hardware can talk to our software.

Next, essential system processes and user space items are launched.

<img width="1272" height="556" alt="image" src="https://github.com/user-attachments/assets/a5aef4de-7755-4ac8-8e8e-b74d1af17a02" />

These include processes like user login, spinning up a desktop environment, and more which basically allows us to interact with our system.
