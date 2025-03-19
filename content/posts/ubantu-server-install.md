---
title: "Install Ubuntu Server"
date: 2025-03-19
draft: false
author: "Nikhil Jayammagari"
avatar: "/img/nikhil.png"
cover: "https://i.postimg.cc/vZqfRgNg/ubantu-server.png"
categories:
  - installation
tags:
  - ubantu-server
  - ubantu
  - homelab
summary: Ubuntu Server is a powerful, open-source operating system designed for servers. It offers stability, security, and flexibility, making it ideal for web hosting, cloud computing, and enterprise environments.
---

**1. Overview**

Ubuntu Server is a variant of the standard Ubuntu you already know, tailored for networks and services.

Unlike the installation of Ubuntu Desktop, Ubuntu Server does not include a graphical installation program. Instead, it uses a text menu-based process. If you’d rather install the desktop version, take a look at our [Install Ubuntu desktop](https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview) tutorial.

This guide will provide an overview of the installation from a USB flash drive.

**2. Requirements**

You’ll need to consider the following before starting the installation:

- Ensure you have at least 2GB of free storage space.
- Have access to a USB flash drive containing the version of Ubuntu Server you want to install.
- If you’re going to install Ubuntu Server alongside data you wish to keep, ensure you have a recent backup.

Checkout This [tutorial](https://ubuntu.com/tutorials?topic=server) that explain how to create an Ubuntu USB flash drive.

**3. Boot from install media**

To trigger the installation process, perform the following:

1. Insert the USB stick or other install media.
2. Restart your computer.
3. Go to BIOS and Disable Secure Boot and Enable UEFI.
4. Boot From Usb Drive.

After a few moments, you should see messages like those shown below on the screen…

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/1/17ee449b2bd7c530d2f996215407fca5b722dcb2.png)

If you are still having problems, check out the [Ubuntu Community documentation on booting from CD/DVD/USB](https://help.ubuntu.com/community/BootFromCD).

**4. Choose your language**

After the boot messages appear, a ‘Language’ menu will be displayed.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/e/e1d75e3584b6a3c23da39263fbf2f9ba6411de9a.png)

As the message suggests, use the Up, Down and Enter keys to navigate through the menu and select the language you wish to use.

**5. Choose the correct keyboard layout**

Before you need to type anything in, the installer will next display a menu asking you to select your keyboard layout and, if applicable, the variant.

![ubantu](https://web.archive.org/web/20240917185516/https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/5/5c918dc341d92f647d6f1665ed2714922d5e688c.png)

If you don’t know which particular variant you want, just go with the default – when Ubuntu Server has been installed you can test and change your preferences more easily if necessary.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/1/150b56850da9ca443d2a4842104ada1c1dfc264c.png)

**6. Choose your install**

Now we are ready to select what you want to install. There are three options in the menu:

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/7/7e92f38c56ca7b2fbb8323d51d6ee35457fe4fce.png)

The bottom two options are used for installing specific components of a Metal As A Service (MAAS) install. If you are installing MAAS, you should check out the [MAAS documentation](https://docs.maas.io/) for more information on this! The rest of this tutorial assumes you select the first option, Install Ubuntu.

**7. Networking## 

The installer will automatically detect and try to configure any network connections via DHCP.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/f/f3e24675ada8dec595905d3853766afdbe1a9039.png)

This is usually automatic and you will not have to enter anything on this screen, it is for information only.

**8. Configure storage**

The next step is to configure storage. The recommended install is to have an entire disk or partition set aside for running Ubuntu.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/4/48e6067fea81202b132da004d467ec9df20ecf4f.png)

If you need to set up a more complicated system, the manual option will allow you to select and reorganise partitions on any connected drives.

**9. Select a device**

This menu will allow you to select a disk from the ones detected on the system.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/5/5be59d8fb261e3f4ed175d11fb660248c9215823.png)

To help identification, the drives will be listed using their system ID. Use the arrow keys and enter to select the disk you wish to use.

**10. Confirm partitions**

With the target drive selected, the installer will calculate what partitions to create and present this information…

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/5/5a1d73b678c2cdbd0a75225d0a583eb156e1b953.png)

If this isn’t what you expected to see (e.g., you have selected the wrong drive), you should use the arrow keys and enter to select Back from the options at the bottom of the screen. This will take you back to the previous menu where you can select a different drive.

It is also possible to manually change the partitions here, by selecting Edit Partitions. Obviously you should only select this if you are familiar with how partitions work.

When you are happy with the disk layout displayed, select Done to continue.

**11. Confirm changes**

Before the installer makes any destructive changes, it will show this final confirmation step. Double check that everything looks good here and you aren’t about to reformat the wrong device!

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/c/c33fb0d6b4b9bfcb982eda42b21ced5187c38e7b.png)

**12. Set up a Profile**

The software is now being installed on the disk, but there is some more information the installer needs. Ubuntu Server needs to have at least one known user for the system, and a hostname. The user also needs a password.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/2/22deb8bda1b7df8dc94a19f6a23bb07c5b7664b0.png)

**13. Install software**

Once you have finished entering the required information, the screen will now show the progress of the installer. Ubuntu Server now installs a concise set of useful software required for servers. This cuts down on the install and setup time dramatically. Of course, after the install is finished, you can install any additional software you may need.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/4/4108bb9cbe9a52f5b39d266e78e0cf2668f58d80.png)

**14. Installation complete**

When the install is complete, you will see a message like this on the screen.

![ubantu](https://ubuntucommunity.s3.us-east-2.amazonaws.com/original/2X/c/c36b4880b5e4291ca57e6a51b527c05449fec48e.png)

Remember to remove the install media, and then press enter to reboot and start the server. Welcome to Ubuntu!

**Congratulations You Have Successfully installed Ubuntu Server**
