# Ubuntu VM Creation

This is how to create an ubuntu vm.

Use VirutalBox (or VMware if you want to do this)

This is what you need:
* Windows 10 Laptop 
* virtualbox vm (see download link below)
* ubuntu iso (see download link below)


Downloads
-------
### Ubuntu ISO
1. Go to the ubuntu download site
https://ubuntu.com/download/desktop
2. Scroll down to where it says Ubuntu 19.04 and download
3. Make sure you get 64bit and not 32bit
4. It might take a bit because it is a larger file


### VirtualBox
1. Go to VirtualBox site and download 
https://www.virtualbox.org/
2. Install virtualbox onto your system


VM Creation
-------------
1. Open VBox and click `New`
2. Click `Next`
3. Enter a name for your VM (e.g. `Ubuntu`) and set the Operating System to `Linux` and version to `Ubuntu` (64-bit)
4. If CPU virtualization technology (VT-x AMD/V) is not already setup in your BIOS then do it now. (See link below)
https://askubuntu.com/questions/256792/how-do-i-enable-hardware-virtualization-technology-vt-x-for-use-in-virtualbox
5. Enter RAM for VM (probably set to 3-4 GB = `3000-4000 MB`) 
6. Keep default options and click `Next`
7. Click `Next` again
8. Click `Next` again
9. Give your VM at least `30GB` of storage
10. Click `Create`
11. Make sure `Ubuntu` is selected in the list and press `Start`
12. Click `Next`
13. Click on the little folder icon and then navigate to the `Ubuntu 19.04 ISO` file we downloaded earlier
14. Click `Start`
15. After successful install need to remove installation media. Click on `Devices` menu and go to the little disk dvd menu and select the `iso` file from the list and remove it
16. For good measure once in restart 
17. Once restarted run the following commands:
```bash
sudo apt-get update && apt-get upgrade
```
(Note: it will prompt you with a password to use sudo. Just enter the password you setup and press enter. Also note: When you type a password it will not show up so you won't see that you are typing but you are)
18. Enjoy!



