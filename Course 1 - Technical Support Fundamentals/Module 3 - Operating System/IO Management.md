[I/O Management](https://www.youtube.com/watch?v=TPjqviaozdw)

We refer to devices that perform **input and output as I/O devices**.

<img width="1269" height="299" alt="image" src="https://github.com/user-attachments/assets/dd8be701-2de2-4f4a-9b83-8d1c4d92aa2b" />

These include our monitors, keyboards, mice, hard disk drives, speakers, Bluetooth headsets, 
webcams and network adapters.

These I/O devices are all managed by our kernel, the kernel needs to be able to load
up drivers that are used so that we can recognize and speak to these different types of hardware.

When the kernel is able to start the drivers to communicate with hardware, it also manages the transfer 
of data in and out of the devices.

<img width="1239" height="676" alt="image" src="https://github.com/user-attachments/assets/d71d7c8b-4044-434e-832f-5e0f914e9d79" />


I/O doesn't just mean the transfer of data between us and our devices.

The devices also need to be able to talk to each other.

Our kernel handles all the inter communication between devices.

It also figures out what the most efficient method of transfer is and it tries its best to make sure our data doesn't have errors during process.

When you're **troubleshooting** or **solving a problem** with a slow machine it's usually some sort of hardware resource deficiency.

If you don't have enough RAM you can't load up as many processes.

If you don't have enough CPU you can't execute programs fast enough.


<img width="1278" height="347" alt="image" src="https://github.com/user-attachments/assets/2aaec341-5b18-4371-a9a4-fbda35a82f7d" />


If you have too much input coming into the device or too much output going somewhere you'll also block other data from being sent or received.

It's slow is one of the most common problems you'll solve.

Knowing the potential sources of that slowness is a big help when you're trying to narrow down the cause of the latency.

**Troubleshooting** is such an important part. 
