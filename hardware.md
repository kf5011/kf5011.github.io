---
layout: default
---

# FRDM K64F

# Mbed Applications Shield
 * [Board's page in the mbed site](https://developer.mbed.org/platforms/FRDM-K64F/)
 * [NXP page with links to technical docs](http://www.nxp.com/products/software-and-tools/hardware-development-tools/freedom-development-boards/freedom-development-platform-for-kinetis-k64-k63-and-k24-mcus:FRDM-K64F)
# Windows 10 Fix
Windows 10 seems to mess with the board reset.  The problem lies in that Windows is trying to write drive house-keeping data to the virtual usb drive that appears as "MBED" (folders like _System Volume Information_).

Looking through various forums, this looks like a common complaint.
Most of the recommended solutions to turn off this feature involve setting a registry-key **DisableAutomaticRemovableDriveIndexing** to 1.

I didn't have any success with that, but the following comment I found in one discussion fixed the issue.  I now have my version of Windows 10 playing nicely with the board. (http://disq.us/p/15vrugs)
> In recent versions of Windows 10, as well as the above, you need to stop the Storage Service too (type Services into the start menu to find the management applet)

# If you do something silly
> Like press the reset button while running a debugger.

And end up with the red and green lights stuck on

* [https://developer.mbed.org/handbook/Firmware-FRDM-K64F](https://developer.mbed.org/handbook/Firmware-FRDM-K64F)
* [Recovering FRDM-K64F mbed Board](https://mcuoneclipse.com/2014/04/19/recovering-frdm-k64f-mbed-board/)
* [How to Recover the OpenSDA V2.x Bootloader](https://mcuoneclipse.com/2016/06/26/how-to-recover-the-opensda-v2-x-bootloader/)
* [Firmware FRDM K64F](https://developer.mbed.org/handbook/Firmware-FRDM-K64F)
* [Download – OpenSDA Bootloader and Application](http://www.nxp.com/products/software-and-tools/run-time-software/kinetis-software-and-tools/ides-for-kinetis-mcus/opensda-serial-and-debug-adapter:OPENSDA?tid=vanOpenSDA#FRDM-K64F)
* [OPENSDA: OpenSDA Serial and Debug Adapter](http://www.nxp.com/products/software-and-tools/run-time-software/kinetis-software-and-tools/ides-for-kinetis-mcus/opensda-serial-and-debug-adapter:OPENSDA?tid=vanOpenSDA)


# Documentation
I've collected all the technical documentation and datasheets I can find.
(I'll have to go back and find the urls)

## ARM Cortex M4
* [Cortex M4 Generic User Guide](docs\DUI0553A_cortex_m4_dgug.pdf)

## FRDM K64F
* [FRDM K64F User Guide](docs/FRDMK64FUG.pdf)
* [K64F processor Reference Manual](docs/K64P144M120SF5RM.pdf)
* [Accelerometer and Magnetometer](docs/FXOS8700CQ.pdf)
* [RGB led datasheet](docs/CLV1AFKB(874).pdf)
* [Board Schematic](docs/FRDM-K64F-SCH-E4.pdf)
* [Headder pins](docs/FRDM-K64F_PKG_pins.pdf)

## Application Shield
* [Board Schematic](docs/ApplicationShield V_1_0_0 SCH.pdf)
* [Board PCB layout](docs/ApplicationShield V_1_0_0 BRD.pdf)
* [LCD Datasheet](docs/NHD-C12832A1Z-FSW-FBW-3V3.pdf)
* [5-way switch](docs/SKRH Series - Basic information.pdf)
* [RGB led datasheet](docs/CLV1AFKB(874).pdf)
* [Accelerometer](docs/MMA7660FC.pdf)
* [Temperature sensor](docs/LM75B.pdf)
