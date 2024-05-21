# thinkpad-x280-hackintosh
a tutorial and a boot efi for thinkpad x280 hackintosh, with all drivers for macOS.

## step1
install python on your computer.

## step2
run macrecovery.py

macrecovery.py -b Mac-E43C1C25D4880AD6 -m 00000000000000000 download

notice: mac os list, https://github.com/acidanthera/OpenCorePkg/blob/master/Utilities/macrecovery/recovery_urls.txt, please select a suitable os, or use the default code above.


## step3

A. After starting the download, the BaseSystem.chunklist and BaseSystem.dmg files will be downloaded to your computer;

B. Prepare a USB drive and format it in regular Fat32 format;

C. Create a folder named com.apple.recovery.boot in the root directory of the USB drive, without any errors;

D. Copy the downloaded BaseSystem.chunklist and BaseSystem.dmg folders to the USB drive;

E. Set a startup name for Recovery and create a new text file in the com.apple.recovery.boot file; Open the newly created text file and enter the startup name you want, which can be filled in freely. You will enter "Big sur 11.2.3"(this name is just a label, whatever it is), which will appear in the OC startup interface. Then, change the file name to .contentDetails and set it as a hidden file;

F. Put the EFI file booted by OpenCore into the root directory of the USB drive;

G. The EFI folder is at the same level as com.apple.recovery.boot, so do not put com.apple.recovery.boot in the EFI folder;

At this point, the deployment of the Recovery online installation tool has been completed. As long as you configure the OpenCore EFI driver that belongs to your computer, you can use this Recovery to install black Apple systems on various computers.


Turn on the computer, select USB flash drive UEFI to start, and then select "Big sur 11.2.3" to enter the Recovery tool.

# About The EFI
I have installed few times for my thinkpad x280, and have fixed some drivers and add some drivers, now the EFI can be work very well for thinkpad x280, every driver is ok, but it has no "airdrop" because the machine has no hardware to support it.

Enjoy!