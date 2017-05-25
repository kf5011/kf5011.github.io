---
layout: default
---

# FRDM K64F

# Mbed Applications Shield
[Board's page in the mbed site](https://developer.mbed.org/platforms/FRDM-K64F/)
[NXP page with links to technical docs](http://www.nxp.com/products/software-and-tools/hardware-development-tools/freedom-development-boards/freedom-development-platform-for-kinetis-k64-k63-and-k24-mcus:FRDM-K64F)
# Windows 10 Fix
Windows 10 seems to mess with the board reset.  The problem lies in that Windows is trying to write drive house-keeping data to the virtual usb drive that appears as "MBED" (folders like _System Volume Information_).

Looking through various forums, this looks like a common complaint.
Most of the recommended solutions to turn off this feature involve setting a registry-key **DisableAutomaticRemovableDriveIndexing** to 1.

I didn't have any success with that, but the following comment I found in one discussion fixed the issue.  I now have my version of Windows 10 playing nicely with the board. (http://disq.us/p/15vrugs)
> In recent versions of Windows 10, as well as the above, you need to stop the Storage Service too (type Services into the start menu to find the management applet)
