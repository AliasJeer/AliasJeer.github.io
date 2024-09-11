---
layout: single
title:  "Switching to Linux"
date:   2024-09-01 23:27:31 -0500
categories: Linux, Operating Systems, Cybersecurity
author: AliasJeer
header: 
    image: /assets/images/parrot-desktop-screenshot.png
    teaser: /assets/images/parrot-desktop-screenshot.png
---
## The time has come 
After years of "playing" with Linux in virtual machines, live USBs, and online boxes, I decided to take the plunge and install Parrot OS on the bare metal of my laptop. This decision was something I had been thinking about for a long while as I increasingly grew tired of the tedium of booting multiple machines. I had previously been using Windows on the bare metal and using a portable SSD to boot a Parrot live install when I wanted it. One of the main reasons I decided to switch is because the SSD was basically always plugged in and it got tedious dealing with the cable and drive flopping around.

At the same time recent Windows updates and security flaws have left me wondering why I am even bothering with Windows anyway. I never use it and I have no real need for it. It is just familiar.

**Familiar is no longer enough.**

When lime mentioned she was thinking about switching too I was even more certain the time had come. We loaded up the installed on a flash drive and jotted down the windows product and activation keys. I doubt I will ever need them, as I will describe more later, but just in case, I had my safety net. Time to do this.

## Why Parrot?
There are many Linux distributions to choose from, some more purpose built and some made for general use. While many in cybersecurity will recommend Kali as the standard, I chose Parrot for a few reasons:
- It's familiar (I know I know) from my coursework at HTB Academy
- Lightweight and actively in development
- Comprehensive security tool set
- It just plain looks good

With all that said, let's get to the meat of this bone.
## Creating the live boot installer
Navigate to https://www.parrotsec.org/download/ and select your version. If you are installing on your laptop or dual booting, you will select the Live option. I chose the Security edition because I plan to use this install as a daily driver for my cybersecurity training and career. 

After verifying the checksums, I opened up Balena Etcher and selected the Parrot ISO and the flash drive and hit "Flash!". When it was finished, I rebooted my computer and said goodbye to Windows. Hitting the key to bring up the boot options (F12 for me) I selected the USB and loaded up Parrot. I immediately clicked on the "Install Parrot" icon and got started going through the installer. 

After selecting all the options, I chose "Swap to File" and then proceeded to REALLY say goodbye to Windows by overwriting the partition. When it was finished, I rebooted and got ready to become an official Linux user.

## Setting things up
I was amazed at how quickly the system booted with the fresh Parrot install. Everything was crisp, properly scaled and looking amazing. After a few minutes of poking around I started the inevitable task of customizing the look and feel. The native MATE desktop is clean and simple and the options for customization, while somewhat limited, can still give you the chance to make the environment your own. I selected a background image and customized the theme a bit and got down to trying everything out.

On lime's advice I pulled up Firefox and went to Youtube to check out a 4K video. Everything looked crisp and rendered well, telling me that the video drivers were correctly installed. So far so good!

## One little issue
When I closed the lid which is supposed to suspend, and then logged back into it later, the WiFi would not connect. Furthermore it could not be re-enabled until the system was rebooted. Manually suspending or using the power button to suspend had the same issue. 

I checked drivers, I checked settings, I checked myself. Nothing seemed to resolve the issue. Restarting Network Manager had no effect. Finally I remembered that while using the SSD bootable, I had to change the sleep settings in the BIOS to allow the sleep function to work properly running off the connected drive. I had switched it from Windows to "LinuxS3" which worked on the bootable SSD but I had to switch it back to "Windows/Linux" to avoid the loss of wifi issue.

I'm sure there is a more elegant long term fix for this that would still allow me to use the S3 sleep but for now at least I can shut the lid when I take a break and come back to work without having to reboot. 

## I love it
For me this has been one of my favorite decisions of the year. Parrot is a very comfortable environment and seems incredibly stable. It strikes a nice balance automating some of the more tedious management tasks but leaving a lot to explore and learn. Everything seems to run really well and the shutdown and bootup are the fastest I have ever experienced on any computer or OS. I look forward to learning more and I don't think I'll ever go back to Windows.