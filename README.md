<img src="https://filebox.ece.vt.edu/~jbhuang/images/vt-logo.png" width="240" align="right">  

Install Window 10 and Ubunt 18.04  on MacBook Pro  
by Jianyuan (Jet) Yu  
jianyuan@vt.edu 

# Prequisiste
* windows .iso
* Ubuntu .iso
* 16G usb flash disk
* **balenaEtcher** - tool to flash ISO into disk

# MacOS
Machine: Macbook Pro 2013 or 2015.  
OS: version 10.13 High Sierra  
Note for version 10.15 Catalina, skip step A.2-5  

  

# A. Install Windows
1. In MacOS use the **Boot Camp Assistant**, it will create a OSXRESERVED partition and fail at "An error occurred while copying the Windows installation files "
2. follow the solution [ref solution](https://discussions.apple.com/thread/8633033): (a).Use Disk Utility to erase the newly created “OSXRESERVED” partition, and with the erase feature, choose the ExFAT Format. (This format will allow you to write larger files than the FAT 32 format) (b).Manually copy all the contents from the Windows 10 ISO to the OSXRESROUCES volume.
3. 1st restart your Mac, hold **opt** key to start the Windows
4. you will see lot of drivers (include wifi) not installed
5. 2nd restart machine boot into MacOS, [Download and install Windows support software on your Mac](https://support.apple.com/en-us/HT204923) to install driver on a usb disk
6. 3rd restart machine into Windows, install these drivers from the disk, then all set



# B. Install Unbuntu (based on Window)
1. flash Ubuntu iso file into disk using **balenaEtcher** 
2. reboot machine, choose the disk to continue
3. click split the windows disk and continue



# Issue
1. cannot launch window after install Ubuntu, potential solution [boot repair](https://help.ubuntu.com/community/Boot-Repair), [2](https://itectec.com/ubuntu/ubuntu-repair-windows-boot-loader-after-installing-ubuntu-on-macbook-pro/)
