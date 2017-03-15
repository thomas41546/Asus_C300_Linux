## Summary
This repository has essential files for installing a fully functional Asus C300 Chromebook Linux System

## Bios and Install
Remove write-protect screw from Asus C300 Chromebook motherboard, http://www.matws.org/c300/

Get Developer Access on Chromebook

Open Console

Install SeaBios via /bios/lewis-fw-c300.tar.gz script

Install your OS choice on a USB drive (MBR boot), I used Linux Mint 17.2

Boot into your USB and install it to the MMC 16GB, be very careful not to touch the boot MMC.

## Kernel
Under the /kernel directory is a bash script that will install Linux 4.4 32 bit, this version has the best support for the C300.

Keyboard, Touchpad, Wifi, Sleep, Screen Brightness, Sound all work if you do the work below with this kernel.

## Sound
Copy the fw_sst* files to /lib/firmware/intel/

Copy the asound.state to /var/lib/alsa.asound.state

Reboot

## Wifi
Copy iwlwifi-7260-17.ucode /lib/firmware

Reboot

 
