# Headless-Raspberry-Pi-4-Kali-GNU-Linux-
Draft:

In this repository I'm going to explain how to install Kali Linux on a Raspberry Pi 4 without display (Headless) using SSH to connect the other computer.

sudo apt install xz-utils
unxz IMAGEDISK_HERE.img.xz


sudo apt install gddrescue 
or
sudo apt install ddrescue
sudo apt -get ddrescue



sudo ddrescue -D --force IMAGEDISK_HERE.img /dev/sdb 

or 

dd bs=4M if= IMAGEDISK_HERE.img of=/dev/sdb

sync

Now go to cd /etc/NetworkManager/system-connections in your computer and copy the "Wired connection 1" file or something similar

Now is time to go to 

ROOTFS/etc/NetworkManager/system-connections paste "Wired connection 1" you can use touch and then nano to modifi the file

then go to /etc/network/___
then go to /etc/lightdm/___

modifi


