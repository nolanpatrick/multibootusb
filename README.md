# multibootusb
This repository consists of config files and other things necessary to create a USB stick capable of booting multiple operating systems in live mode using the GRUB2 bootloader.

WARNING and DISCLAIMER: This will destroy all data on the target USB drive and may cause data loss on other disks if you pick the wrong drive during setup. I am not responsible for any loss of data or other problems associated with this project.

1. To begin you must create a new MSDOS partision table on the drive you would like to use. This will wipe all data on the USB disk so make sure you back up anything important.

2. Next you need to create a single ext4 partition spanning the whole drive. "/dev/sdax" is the drive enumeration of your USB stick. It is important to choose the correct one.
```bash
# mkfs.ext4 /dev/sdx1
```
