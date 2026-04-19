# Installing, Updating and Removing Software in Linux

### What you'll do

**Update**- The machine you'll be using comes preinstalled with an old version of the VLC Media Player. You'll update VLC to the newest version.

**Install**- You'll install the Mozilla Firefox web browser. There's currently no version of Firefox on the machine you'll be using, so it will be a fresh installation.

**Uninstall** - You'll uninstall the GIMP photo-editing tool from the machine, removing it entirely.


## Verifying installed software on Linux

To quickly check if a program is installed on Linux, you can use the command "**dpkg -s"** followed by 
the unique package name for that program. The "**-s**" flag in dpkg **stands for "search**," which allows you 
to search for a program on your machine and check if it's installed. For example, we know that Firefox 
isn't currently installed, but GIMP is. Running "**dpkg -s firefox-esr**" shows this output:

```
dpkg -s firefox-esr

```
#### Output:

```
dpkg-query: package 'firefox-esr' is not installed and no information is available
Use dpkg --info (= dpkg-deb --info) to examine archive files.

```

This shows you that Firefox isn't currently installed on the system. To check GIMP, modify the earlier command and enter "dpkg -s gimp" to see the output below. (Note that only part of the output is shown.)

```
dpkg -s gimp

```
#### Output:

```
Package: gimp
Status: install ok installed
Priority: optional
Section: graphics
Installed-Size: 19016
Maintainer: Debian GNOME Maintainers < pkg-gnome-maintainers@lists.alioth.debian.org >
Architecture: amd64
Version: 2.10.8-2+deb10u1
Replaces: gimp-plugin-registry (<< 7.20140602+nmu1~)
```

You can see that the status of **gimp** is "installed". As long as you know the package name, 
you can use "dpkg" to check the status of any program.

Running "dpkg -s vlc" shows you that vlc is installed, but also that the version is out-of-date. 
(Version 2.2.7 is installed, but the newest version is at least 3.0.12)

```
dpkg -s vlc


```

#### Output:

```
Package: vlc
Status: install ok installed
Priority: optional
Section: video
Installed-Size: 4667
Maintainer: Debian Multimedia Maintainers < pkg-multimedia-maintainers@lists.alioth.debian.org >
Architecture: amd64
Version: 2.2.7-1~deb8u1
```

## Updating VLC Media Player

VLC media player is already installed on your computer, but the version that's installed is out-of-date.
You'll fix that now by **updating** it to the **newest version**. To do that, force an update of the package manager, 
using this command:

```
sudo apt-get install -f
```

This kicks off the update process. It will print out lots of text to your terminal, and ask you 
if you'd like to continue. Enter "y" for "yes". When the process is finished, type "dpkg -s vlc" 
again to verify the installation.

```
dpkg -s vlc

```

#### Output:
```
Package: vlc
Status: install ok installed
Priority: optional
Section: video
Installed-Size: 231
Maintainer: Debian Multimedia Maintainers < debian-multimedia@lists.debian.org >
Architecture: amd64
Version: 3.0.20-0+deb10u1
Provides: mp3-decoder
```


You can see here that VLC has been updated to a newer version (3.0.12 was the newest at the time this screenshot was taken). Your version should be at least 3.0.12, but could be higher if newer versions have been released.

## Installing Mozilla Firefox

Let's install the Mozilla Firefox web browser. Parts of this process will be unique to this specific installation, but most of the steps you'll take will be identical, regardless of the software.

Lots of common programs, including Firefox, are set up in repositories that most Linux distributions are aware of, by default. This makes installing these programs super easy, and allows you to bypass having to manually download and install the program. To make sure these repositories are up-to-date and all dependencies are fixed, run the below command into the terminal (you will have to enter the letter "Y" at some point during the process to confirm your action):

```
sudo apt-get update

```

This will start the repository update process, which should look something like this when it's finished:

#### Output:
```
Hit:1 http://deb.debian.org/debian buster InRelease
Hit:2 http://deb.debian.org/debian-security buster/updates InRelease
Hit:3 http://deb.debian.org/debian buster-updates InRelease
Reading package lists... Done
```


Now you're ready to install Firefox. Run the below command in the terminal:

```
sudo apt-get install firefox-esr

```

You'll be prompted to confirm that you‘d like to continue with the installation. To continue, enter "y" (as in "yes") into the terminal, and hit "enter". For future reference, to cancel the installation process, you'd just enter anything other than "y".

#### Output:

```
Reading package lists... Done
Building dependency tree       
Reading state information... Done

The following additional packages will be installed:
  libdbus-glib-1-2
Suggested packages:
  fonts-stix | otf-stix fonts-lmodern libcanberra0 pulseaudio
The following NEW packages will be installed:
  firefox-esr libdbus-glib-1-2
0 upgraded, 2 newly installed, 0 to remove and 56 not upgraded.
Need to get 62.7 MB of archives.
After this operation, 235 MB of additional disk space will be used.
Do you want to continue? [Y/n]

```


After confirming the installation, the terminal will briefly fill with lines of text. Once this process is complete, Firefox will be installed on your instance. To verify that it's installed, enter "dpkg -s firefox-esr" into the terminal window again, and you'll see different output than before:

```

dpkg -s firefox-esr

```

#### Output:

```
Package: firefox-esr
Status: install ok installed
Priority: optional
Section: web
Installed-Size: 229154
Maintainer: Maintainers of Mozilla-related packages < team+pkg-mozilla@tracker.debian.org >
Architecture: amd64
Version: 115.11.0esr-1~deb10u1
Provides: gnome-www-browser, www-browser
```

You can see that the status is listed as "installed", meaning that the process was successfully completed. Wohoo! Now you can move onto updating software.

## Uninstalling GIMP

When it's no longer necessary to have a specific program installed on your computer, it's usually a good idea to uninstall it to clear up space. Now, you'll uninstall the GIMP photo-editing software, removing it from the computer completely.

GIMP, like Firefox, can be i**nstalled and uninstalled** using the "**apt-get**" commands that you used to install Firefox. To uninstall GIMP, a very similar command is used:

```
sudo apt-get remove gimp
```

This command will kick off the process of uninstalling GIMP from your instance. Shortly after starting, it will prompt you to confirm the uninstallation. Enter "y" to confirm, and the process will begin:

#### Output:

```
The following packages will be REMOVED:
  gimp
0 upgraded, 0 newly installed, 1 to remove and 56 not upgraded.
After this operation, 19.5 MB disk space will be freed.
Do you want to continue? [Y/n] Y
```

After receiving your confirmation, the process will continue and GIMP will be uninstalled. You can verify that the process was successful by running the same command we used to verify its installation ("dpkg -s gimp"). You'll receive the following message. (Only part of the message is shown below.) Note the this message shows that GIMP has been "deinstalled".

```
dpkg -s gimp

```

#### Output:

```
dpkg-query: package 'gimp' is not installed and no information is available
Use dpkg --info (= dpkg-deb --info) to examine archive files.

```
This confirms that GIMP was successfully removed from your computer.
