---
title: "How to Install Proxmox VE"
date: 2025-03-10
draft: false
author: "Nikhil Jayammagari"
cover: proxmox-ve-install.png
---

Proxmox VE is an open-source server platform for enterprise virtualization. As a Debian-based Linux distribution, Proxmox uses a modified Ubuntu kernel to run multiple virtual machines and containers on a single server. You can deploy and manage virtualized environments through a web console or a command line, ensuring simple and fast accessibility.

Prerequisites

A physical or dedicated server.
64bit CPU.
At least 1GB of RAM (and additional RAM needed for guests).
A USB stick with at least 1GB.
Install Proxmox Virtual Environment
Follow the steps below to install Proxmox VE on a physical or dedicated server.

Step 1: Download Proxmox ISO Image
The first step is to download the Proxmox VE ISO image.

1. Navigate to the official Proxmox Downloads page and select Proxmox Virtual Environment.

Proxmox download page.
2. This takes you to the Proxmox Virtual Environment Archive, which stores ISO images and official documentation. Select ISO Images to continue.

Open Proxmox ISO images achieve. 
3. At the time of writing, the latest version of the Proxmox VE ISO Installer is 7.1. If a newer version is available, it is listed at the top. Click Download and save the file.

Download the latest Proxmox VE ISO installer.
Step 2: Prepare Installation Medium
Copy the Proxmox ISO image on a CD/DVD or a USB flash drive. Although both options are possible, it is assumed that most systems won’t have an optical drive.

Plug in the USB drive and copy the ISO image to the USB stick using the command line or a USB formatting utility (such as Etcher or Rufus).

Step 3: Launch the Proxmox Installer
1. Move to the server (machine) where you want to install Proxmox and plug in the USB device.

2. While the server is booting up, access the boot menu by pressing the required keyboard key(s). Most commonly, they are either Esc, F2, F10, F11, or F12.

3. Select the installation medium with the Proxmox ISO image and boot from it.

4. Next, the Proxmox VE menu appears. Select Install Proxmox VE to start the standard installation.

Proxmox installer menu.
5. Read and accept the EULA to continue.

Proxmox EULA.
6. Choose the target hard disk where you want to install Proxmox. Click Options to specify additional parameters, such as the filesystem. By default, it is set to ext4.

Select Proxmox target hard disk.
7. Then, set the location, time zone, and keyboard layout. The installer autodetects most of these configurations.

Configure location and timezone for Proxmox.
8. Create a strong password for your admin credentials, retype the password to confirm, and type in an email address for system administrator notifications.

Set administration password for Proxmox.
9. The final step in installing Proxmox is setting up the network configuration. Select the management interface, a hostname for the server, an available IP address, the default gateway, and a DNS server. During the installation process, use either an IPv4 or IPv6 address. To use both, modify the configuration after installing.

Management network configuration.
10. The installer summarizes the selected options. After confirming everything is in order, press Install.

11. remove the USB drive and reboot the system after installation.

Step 4: Run Proxmox
1. Once the system reboots, the Proxmox GRUB menu loads. Select Proxmox Virtual Environment GNU/Linux and press Enter.

2. Next, the Proxmox VE welcome message appears. It includes an IP address that loads Proxmox. Navigate to that IP address in a web browser of your choice.

Proxmox welcome output.
3. After navigating to the required IP address, you may see a warning message that the page is unsafe because Proxmox VE uses self-signed SSL certificates. Click the IP link to proceed to the Proxmox web management interface.

Accept proxmox certificate and proceed.
4. To access the interface, log in as root and provide the password set when installing Proxmox.


5. A dialogue box pops up saying there is no valid subscription for the server. Proxmox offers an optional add-on service to which you can subscribe. To ignore the message, click OK.


Step 5: Create a VM
Now that you logged in to the Proxmox web console, follow these steps to create a virtual machine.

1. Before going through the steps to create a virtual machine, make sure you have ISO images for installation mediums. Move to the resource tree on the left side of your GUI.

Select the server you are running and click on local (pve1). Select ISO Images from the menu and choose between uploading an image or downloading it from a URL.

Add ISO images to Proxmox VE.
2. Once you have added an ISO image, spin up a virtual machine. Click the Create VM button.

Start creating a VM on Proxmox.
3. Provide general information about the VM:

Start by selecting the Node. If you are starting and have no nodes yet, Proxmox automatically selects node 1 (pve1).
Provide a VM ID. Each resource has to have a unique ID.
Finally, create a name for the VM. Use an easily identifiable name.
General options for setting up a virtual machine.
3. Next, switch to the OS tab and select the ISO image you want for your VM. Define the Type of the OS and kernel Version. Click Next to continue.

Select OS for Proxmox virtual machine.
4. Modify system options (such as the Graphic card and SCSI controller) or leave the default settings.

System options for proxmox.
5. Configure any Hard Disk options you want the VM to have. You can leave all the default settings. However, if the physical server uses an SSD, enable the Discard option.

Hard disk options for Proxmox VM.
6. The number of Cores the physical server has determines how many cores you can provide to the VM. The number of cores allocated also depends on the predicted workload.

Set CPU options for Proxmox virtual machine.
7. Next, choose how much Memory (MiB) you want to assign to the VM.

Configure memory for virtual machine.
8. Move on to the Network tab. It is recommended to separate the management interface and the VM network. For now, leave the default setting.

Configure network options for VM.
9. After clicking Next, Proxmox loads the Confirm tab that summarizes the selected VM options. To start the VM immediately, check the box under the listed information or start the VM manually later. Click Finish to create the VM.

VM summary.
10. See the newly created VM in the resource tree on the left side of the screen. Click on the VM to see its specifications and options.

Proxmox virtual machine.
Congratulations You Have Successfully installed