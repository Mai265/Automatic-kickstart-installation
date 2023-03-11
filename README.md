# Automatic Kickstart Installation
Steps to automate VM installation via webserver using Kickstart.

Machine specifications:
- Memory 2048MB 
- Processores 2
- Hard Disk 40GB
- Network Adapter NAT
- ISO CentOS7

## 1. Install a webserver 
You can see installation and configuration steps in https://github.com/Mai265/Creating-VirtualHosts-over-the-same-webserver-socket .

## 2. Copy Kickstart file
Copy attached Kickstart file to webserver data path `/var/www/ahmed.com/ks.cfg`, and edit it with your root and user passwords. 

## 3. Start new VM
Select the listed specifications and attach centos iso.

## 4. Boot the new VM 
Boot the new VM from ISO, and mdify the installer kernel to use the kickstart from the webserver as shown :
- Select the wanted kernel from boot menu, and press `tab`
- Press `e`, and append the underlined part  
![alt text](https://github.com/Mai265/Automatic-kickstart-installation/blob/main/MicrosoftTeams-image.png)
- press `Enter` to complete installation process

** After the installation the machine will restart automatialy and prompt you to enter the user name and password. **
![alt text]()


