# Setup Debian on VirtualBox

## Step 1: Install VirtualBox and Extension Pack

1. **Install VirtualBox**  
   VirtualBox is free, open-source software for running multiple OS on your computer.  
   [Download VirtualBox](https://www.oracle.com/virtualization/virtualbox/)

2. **Install the Extension Pack**  
   The Extension Pack adds features like USB support and PXE boot.  
   [Download Extension Pack](https://www.oracle.com/virtualization/virtualbox/)

## Step 2: Download the Debian ISO

1. **Download Debian**  
   [Download Debian ISO](https://www.debian.org/)

## Step 3: Create a Virtual Machine

1. Open VirtualBox and click "New" to create a new virtual machine.
2. Select the Debian ISO and proceed with the default settings.

## Step 4: Post-Installation Setup

```bash
su -
usermod -aG sudo <username>
reboot

sudo apt update && sudo apt upgrade -y
sudo apt dist-upgrade -y
sudo apt install -y curl wget git build-essential net-tools
