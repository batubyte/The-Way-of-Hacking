# Kali Linux VM

## Step 1: Install VirtualBox and Extension Pack

1. **Install VirtualBox**  
   VirtualBox is free, open-source software for running multiple OS on your computer.  
   [Download VirtualBox](https://www.oracle.com/virtualization/virtualbox/)

2. **Install the Extension Pack**  
   The Extension Pack adds features like USB support and PXE boot.  
   [Download Extension Pack](https://www.oracle.com/virtualization/virtualbox/)

## Step 2: Install 7-Zip and Import Pre-Made Kali VirtualBox VM

1. **Install 7-Zip**  
   7-Zip is a free tool for compressing and extracting files.  
   [Download 7-Zip](https://www.7-zip.org/)

3. **Install Pre-built Kali VirtualbBox VM**  
   Kali is a Linux distribution used for security testing and hacking.  
   [Download Kali VirtualBox](https://www.kali.org/get-kali/#kali-virtual-machines)
   - Extract VM from zipped file
   - Launch VirtualBox
   - Select ‘Add’, navigate to the location our VM is downloaded and find the .vbox file
   - This image has the default credentials "kali/kali"

## Step 3: Post-Installation Setup

```bash
setxkbmap <keyboard_language>
sudo apt update && sudo apt upgrade -y
sudo apt dist-upgrade -y
sudo apt autoremove -y
sudo apt install build-essential
```
